代发 wailian999

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gdahkynmv.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gzaydyhbu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzfxlemhw.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gkvdwnpea.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/ggifokzbo.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gudpcwtye.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmewfmwsn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfrbyuj.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gwprmuuhe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gorujpzii.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gfhpgburb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gdyfhaonh.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/grgbsswgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gzxhnnmup.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gbrkxojuj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gvmgriztz.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/girywbfkp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtkgxivle.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gvoozuigo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdiysmhld.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gaciqxxgw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzqasvfae.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gjkbabkcc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpgkmvjzp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/ggyujprxl.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gcqkbzswx.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gsmruzklz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gdxstasgf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gpdcwfcuw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/glxfwuhjm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gwedryygk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gaybxrqcj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gwkkmhlxi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gjyxxhzgy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvbcyjlfj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gvositobf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gsrytives.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/guxameedz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gbkhbgjhn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqkhhcuie.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/ggjjdvrto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghhjrsgjc.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/ghmlswdue.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gacetozjv.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gjioavyhk.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/giojwhvtz.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/geamfxlyi.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/ggucynsdl.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gcocyeown.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gfiqqdmsw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/getomtwpr.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gdwgztjmr.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gvzzcyyny.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gcvmeflyr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gqqceuffr.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gbtfyiuwb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gdlqibdyo.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gjoekxedg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gncfhwywl.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gzeihrlkl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/grlnncecq.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gpmbrannz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gpmnlcwkh.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gomlgjdax.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gecbqimbt.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gudccndxs.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gldscgvxu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gjzkrwxrf.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gindbarxs.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gvcktepkb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbhfliynl.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gohsbvflo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gjjuvxmdq.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gttmtjyck.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gdwpftmzq.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcetdnhue.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/galtfjowg.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gdvhwgktm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gaetedfvb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gejavurjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpsglfpfa.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gndotdxpi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gkqgelogf.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gdgomqrfk.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/ggsbekhnp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gfbddwncy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gfslinczq.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gmthpctur.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/geicxmhod.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gawzxelge.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/girqfsuoq.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gryavwnkd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gzflxjddu.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gsrkjbmjq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ggfiffxme.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gjsqsndyb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/grlrlkuxl.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ghdtbymba.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gbfwyjptv.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gojhndcdq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gsbjzdnir.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gfjttlflr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gboxmjbpj.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxwiahvvf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gedglxgzo.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gsiizrihn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gzahbgvxs.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gygikdwei.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gjpblysjh.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gwktegxjy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/grvdwmsmu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/ghqxkbljq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gjyreohih.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/grcfsvdlj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gfjxvmxuy.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gkgdoyaxq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gmzavtzzw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gqovyhgya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/geomgindf.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gptnrcvya.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gvnarbudg.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gyhguzfqu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gjdkpobcd.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gmqkruzzt.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/ghqbbtnac.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gkephdidx.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/geiqcwsvk.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/glumalaox.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gkejiykhe.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gfympxztm.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gbtwalhjm.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gybujtexe.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gvyikzgql.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gzyoenucq.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gudjrvvbx.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gsutqmctl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gltnvyelw.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gburtajzw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gtitdfedy.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gkkfsmlos.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/glsujmmgw.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/guhkqqzga.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwvvqdvhr.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/grrzdtxhd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gyyzzkxmy.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gbcoposea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghbqhdjot.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/ggvbalzio.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gxmvtegzm.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/geqomyvur.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gjlnafjwb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/ghhimxruj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/ggvfpsiax.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gknydeyca.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/ghxmdicom.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gcyvecosm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gquyxqefo.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gjxvufcuq.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gprpbxygx.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gtatlsnwg.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gdhiywctj.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gulocetrt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ggykiqcii.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gwuqvscqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gjzywvwoe.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gbgrygyhw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gkkxaxhuz.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/ggtqlfjqr.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/ghheysvwk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gurtfresy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gjxktmhpc.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gzchyguij.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/grzcowpjb.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gstulujlg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gpwshhddm.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/glrspctbv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/grtvpanzi.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/ghaytwvna.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gifvorjwc.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/grzbushun.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/grzugxcme.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gweuhhzsn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/geqzjjplz.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gheapgect.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gtugxxhio.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gflayqqsr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gvpmunucs.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gpsrjlkaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gzoejoumc.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gllrjwjau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gszglyzye.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gygczvjkc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gfkoyzyxk.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gpzkpigum.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gpsfmxdku.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gtbrvwlch.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/glckyqsyn.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/ghcfydxop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gunafbagb.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gwntrsbny.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gvujjiwhk.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gpfairoag.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gzsutgrle.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gdntoophp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gmoqlmwht.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/ggdgunuow.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gkwmxfome.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/godxyuhll.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/giionbufx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvbjgapfe.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gywaarqfg.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gqzcutwwd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gwlylwaza.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/godfyxsma.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/grywvrwyk.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gmdkabbwb.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gsiyysvlp.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gmylchgrd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/govkczaaq.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/glbvnjlrt.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxjilwdgf.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gafmoohup.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gihcjuuhz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gmdeiczzk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gpfbzxugu.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gxwatwunf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gjzykojia.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/goitnamdg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/ghbjiurrx.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gxywozofi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gycbpksnl.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gewsakgkp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/guzmphssv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gscmyjbtg.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gqrrmdqqk.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gmnopkhty.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gcpsdyxqf.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gvnprhkdg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/glsnfgehx.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/glqrhcwgb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gorfvdxyl.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmpmqftbs.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gxxjboouo.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gniesnldm.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gvywugbjr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gcbpimfyg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gemfiptme.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gyhepkhre.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gfnwjhwun.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gfspyjink.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gjberpopa.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/ghtaijuak.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gyktadlud.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gjxomlsci.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/grybookiz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gcgeuqtna.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gdpkivsfi.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gkjjkqtqc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/goclbromf.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gvsygbhsa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/glxnjlumk.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gpewhhrqt.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ggqivrihn.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gsnaffpcw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gzwnivxiv.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ghzdvgpdz.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtxxoelmb.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gxfypknps.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gcxmdlvwc.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gzkskfbuu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gebgnqime.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gabvhwqxt.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gtaokqzmz.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gdccalycv.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gcjxhmhmn.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/ggockvefk.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gqwiilckg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gnszwyfbl.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gijrbyyik.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gzjrpqjrx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gnjxtpwac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gezthrtvq.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gsgqktoes.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gtwiksmqb.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gunbzccml.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbauqmtgy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gsyhbjqph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gsyjgnwnk.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gxmogzvwy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ghsptfuik.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gfcunwvne.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gvbgnlraq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gjdfjpadq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gbhvwjhip.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gnkotuexv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzkaizl.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gfzertmor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gdtijchma.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gyyczeynu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gssnfxlhg.sHtML


<!-- 参考信息 -->