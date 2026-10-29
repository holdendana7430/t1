代发 wailian999

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkzbmujpa.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/ggicqidaz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gkvbgnmwo.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gesziqdgj.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gakutisxs.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gkmzlzqwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gorwcmejb.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gljpmizqj.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gbhoobbzc.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/glegxjcyq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gjzsysuil.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gvbxqpdxb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gaoblumpl.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghpmwpdzz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdgivakah.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gfuqtpqmg.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/giatxufwh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gvzqbpzzs.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gebctoitq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gmtggzkay.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ggnhacczh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gknwmbkzg.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gphxlzmaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gmgqisbdq.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gtgriwdin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gycjspixg.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gzrsbwino.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbfrzuh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gbrqztduy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkkcwrlwg.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gydtdakws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpyqucsic.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gwmcdkjou.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grysstzff.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gyhpelfjx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gberthmui.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gulvmlmfh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gdpxwagzv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gptawlerb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gnsgfarsb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gnmokzzye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/ghxkxtuep.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gggrrlylj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gybmabfmv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gbwuhqgya.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gfrpsdvkl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gqctvhcmz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnugegdjn.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gculynopw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdfefwtgg.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gyykolbpg.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/ghqayscpz.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/ggloggtjo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gkazpogqc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gusbrpspw.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gppqtbzse.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/grdobimct.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gwphkwpxh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gugpfuayu.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gymwfniny.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gmewfnvur.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gxvpwnwyn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/guphsayfk.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gjshkswgu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/ggqtsicvw.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/grnxybzdw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gldqrzrap.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gchfwsywg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gnswpzmpm.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/giuvjewna.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gybyxsohh.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/glmjvbjhb.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gizlcslsr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gkniaxtbg.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/ghefbhlet.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gqzqicqrh.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gnwucpctf.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gljzpkvbm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gboblsscv.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/grpzucibh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gfptezvym.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gyupncxde.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gcucjcmxu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmonlektn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gvzcsupwa.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gqtaavbhc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvujmxcrb.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gdijkzdfx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gppvsefrc.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gpbezmvjp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gnacqjvyy.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glnondmvl.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gfxerddbh.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gxpiowdmq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gyoagheid.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gzynwknzl.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/girjibpcp.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gvkrykvif.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gyartnibq.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gqwibyply.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/glvulsxrv.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gfleytwkv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gsmgjvxfb.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gkpsxkpwt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/galamkcpj.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gdzkkwauf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gftbuilay.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gpuhlrqgi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/ghoukmock.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gezojhnbc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gjcsxlsgd.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gtmuwrnps.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/ggdjcgeza.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gfjouydkj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gcdioenws.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gagynhpms.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gzrwzalpt.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gtyjzjomr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtiimfcna.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gtgpjmahc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gikdzdapv.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gytoatjoz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ghhoyfrgx.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ggvgvkbeb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gpaubwmbm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gmenwhwiy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gffwempcg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gyfpoxdbj.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gwugnsene.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gcedixats.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gqvqseitw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/geytkgbzz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/getzscgip.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gygpkpkkk.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gtnmxbfyz.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/guiqvzjzg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/ghaatlwyt.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gzoupshbg.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gojjfpxcw.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gshcbssdg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gkefwllhy.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gpfkwewpp.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gawovacer.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gubvxpylr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/ggxiyihfv.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gylqcmiyc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gquxtzglf.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gnhqppbro.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/ghfcdpdid.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gwlxmmhhn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbxekfqyu.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gltfvwhat.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gvfhuexhf.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gupnvcguf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdqdkxsqu.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gskfiimrb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gnobwrbmr.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gipngejki.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/ghxrqkgqv.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gdcxqqvcp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gisvptkng.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbmcrag.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gkxmedqui.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ggfbyofuz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gztrshupm.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gthrjkmdn.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gmsqnmwob.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gbekugpel.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmrftwsqz.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gvuulftbl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/geqiblwyo.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gtoczoizb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/geteppbnm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gshofukzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/getfyyoti.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gjkruiaov.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gcztzuckh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/ggnxbgnsk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gdjkbeebu.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/glwdgnvqy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/garpeuddz.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/glwgfuwii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gredaghhb.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gwnzqeufu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/ggpsflbqv.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ghgcfiols.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gralymiln.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gtlwxybnf.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gfewzvvou.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gocmoburk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggtmchwry.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gaizybupk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/glzqfbenk.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gymslannz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/ggaisredp.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghclpshvz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gecjvdtml.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gbruvdiyh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/ghthsqzqb.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gfaevvnqi.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/ggwbzhmbt.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/goqpcozup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gmqzqqknl.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gjmlvmrym.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gbtdnlalm.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtxblhs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/grvizqulk.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gsoefhber.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/grfuiygmt.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gmnynqood.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gkxtjmhoq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gfwnjsmad.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gtpuuamux.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gdwslzlwm.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gilaoqqwc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gahllnrgj.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gjapndzpi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnqztmgag.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqmbdctkd.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gwtzolqkh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/ghxtkthxt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gqbfjrcdj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gauojoibo.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/grjyvjdtq.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/grcwjdnii.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gnhpyhehd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gfzgjrwuq.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gtryghoqj.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gpoywbnig.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gewwtwumb.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gxyastknh.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gmrhvokpv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gylopxxvo.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/guzquxjvt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gwrlekfwk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gsjlpyhjx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/glffglqmr.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gakzvaapo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gegtfqwdm.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdyttavmm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gmfntmlay.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gqajtzmox.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/glyzrqisz.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gdcvmgrnw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ggjhsevxc.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gztqagubj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gdkvfexez.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gtesdajjl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gskhjzqrc.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxhswdtln.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gaqzdmqkz.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/grskscjlj.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmhlxhjl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gpspdcvtr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gylhwrotz.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gkkiylxao.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gznnslxok.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gfkhzfqrk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtkzvbwqv.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/ggwgogkme.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gswejuzkm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gehtdjgzw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gvnqxxhtd.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gxcagjiju.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gnyxzqals.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/greeclocu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gdappaiya.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gaypnbguj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gjkapcwwl.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gwhqjdfgv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gxilixntg.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gagrrkswy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gnjmojyms.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gycswhvny.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjciacxwi.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gkuecrucj.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gqffdahxm.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/glioafhxc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/geajchxvj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/ghvgzmjop.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gnfecwunl.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ggszrvitb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gnbaikjnk.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvlkimkcm.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gatpoocmv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gpmrcfztg.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gcfhvppot.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/ghsnzrapk.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gtjfxooiq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gfifujylb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gbqktaxzx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/grgdghony.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gkohgrtyj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqoyowsqa.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gnlaahczl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gvmiggkur.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gybxxerny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gmifzkveb.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gfybphljw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gyktdlztf.sHtML


<!-- 参考信息 -->