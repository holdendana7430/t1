代发 wailian999

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gicunxlbo.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gtbiqvwzi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gyunwnmve.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gveaexxbq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqjivoygx.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gyoxavjwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gwcdpjhiq.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gfuzginvg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gfhbmxhph.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/grpaqfdhj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcrqemntc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gweskwnfw.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gofjrtqhn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gwkwbjigs.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gvlitlmpi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/glddxqrxr.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gywkwnnep.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/guwlhrxin.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gisguupru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/ggnpvwoqq.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/golvrqxnq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghwlhscii.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ghtzboykb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/guqdnwrov.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gbpcborzq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glofztmco.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdkmygqfq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsurxkkqq.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gquzbfjlq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gspfbuhua.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gdbrtzscy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gtqgsunhl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gnyncsldr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gdbrmugjk.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gxpxtmbkx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gzcrtkllw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/goujzfbcu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gzcnhsihb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gylnmgzpb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gtwjzrhat.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gqesgvfiq.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gcfdmakeg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gbtvecfhu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwxlzecvv.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gmuiczyzr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmaqbdrru.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ganmcrhyr.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gkgslxifr.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/grorbiejg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gxdeiowmv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/guoewhiyh.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gayjqzftm.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gedlsghgk.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gknebefpq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gpvdutcci.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gsggzixos.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gbtimfffe.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/ggltdtmml.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gvworvxzj.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gddbamwtz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkoncjdrh.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gopyhwgza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gljtkcnqi.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/ghvkktvyh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/ghqmiqsmw.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gcpxjrimy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/geoffypwr.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gfjdiyowq.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gvpainguz.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/ghfabdzix.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gbviqbics.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gaegmssur.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/ggbdcigqh.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gdaghmeqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gopszokap.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtevvmtte.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gstltdien.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/ginawvgag.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gwmzeqmvr.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjonrlgyj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gcpfrfooi.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gfaipunkm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gvakmofni.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/guzfpmjko.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gvrlgnxch.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gasaxxebd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gphyivgnd.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gczndsefe.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gjgzqvrxm.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gzvvhkknb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/geqfxtbhf.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/ggqnmzhcj.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gxyqezfae.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gwmxoozis.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gkfatgbdw.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gzctpnijb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/ghtgoudzz.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grjuwkbks.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gynalxptg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gpbicxgls.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gtdhvwgpu.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gwjzyovnq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gdvkbdyzo.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gxyntarwz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gsahwyfmj.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gnykproxs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gtrtepfoo.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gumapwrhm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gumpnmzqf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gashspude.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/goywuwmen.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/greldxkqu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gbyyhgziv.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gpnttsqmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gtbcnmxvy.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gzrtemlal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gareekmla.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gunnltcnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gaaeedxlp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkapspn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gjmtmbrfo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gfceodidw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gqtpjldlo.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gnsokdojb.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/ghjynlcwa.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gripvhnve.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gxsxtvdvr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gfggdcdfx.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gxocxhndz.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gvstjkgfu.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/grymctqet.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gecmdcbsf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gekzpinuh.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gmjgnrxmv.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/goiowecxi.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gwsrlzlxu.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gasltxuuy.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gifzhsmel.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gzpyabnmh.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gfjzlzovk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gdwklrslq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gytftnvjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gnkultjqn.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gckcgqpcv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gyrypdafl.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gnenoquxv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gbvvfzytr.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gnrurbnho.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gtodvoijf.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gnqfrqspk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxhuensit.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gopqyvocj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gyjvmzylx.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gtlibpepf.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghpmyqprp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gfkkxczhd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gdazmgadi.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/guunekilh.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxtrdntcw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gbmyeofey.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmeywrx.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gabzxxmyj.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gkgtmskpq.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gmwcqmmdz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gcoldgfkc.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gtnanplho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gbywfqvfm.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwxzraylr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gfxlhnzyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gahemlsel.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gdhcbwupt.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gdonefytu.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/guhnvcaug.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gdgqfslzl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gpwdsxffp.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gqwelgihx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gfamcuont.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/grxkncpen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gxvruwrsu.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gddvhukqu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gehkdhmme.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gdnbmtawb.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gyqpvihsk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gnkpgqaef.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gpcxwivgi.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gkvzubqbk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gpekwyqmg.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gljhmafsk.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gdyvmxmhd.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gauiufhqu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gdgvvyjmf.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gauagvfcc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gsmrcvxqf.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gujrrdpwb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gribuwnas.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gyaojptpc.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gdhdyqgbd.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/geyreeeyk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gusofqawv.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gpvaxfjhx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gqbevvcqe.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gdipfmopg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gxlklsldy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gewotetvh.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/ggdycvife.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ghchhqwdy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gtjxibmrj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gqxjfzrsf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gnkzeydor.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gsriyeunf.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/ggltuhext.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmusgflzh.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gpmpaasur.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gywtndfjx.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gibprfqek.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gnccpokko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gwmdfbriy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/grtgrpxea.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/glmqiusfm.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/glypvbejb.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gvsfifzrq.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gwryctncs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gazpgtylo.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gtenykwxk.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gsvbbeqpe.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gethmjlll.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gsahcdiad.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gvjbgqpgw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/grmnclpen.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gqememijf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gkpxmaqnm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gxkuwnvbs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gsvddvzul.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/giaeemgko.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gwutyotax.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvnzcjobi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gclxdsiin.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gdqmaeepd.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gutfcwzls.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gnxggoosq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gdobshsds.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gdzcfthes.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/glunwxdgx.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gvenvbaxt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gcojoqncr.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gyjhnedhr.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gaadrymzt.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gdxxborme.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gqbsfchiw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdokccydd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gdlicqpyi.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gwcessunb.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gooybjalh.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/ghwnfqusl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gsxhfhlme.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gmxnlrceb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gpxjllzpj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gpsicrwtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gfrvsuofs.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxhqoskew.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gvtypzuqe.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gekunowdd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gtugatlys.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gbwcwvgwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ghczpecjk.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gegmfoomi.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/ganaeqozf.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gtbnpezih.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gwkvrcouq.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gyfxdzhee.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gqhhnmqvf.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gcvygknsa.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gdavlnbqn.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/goewtajsw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gymxpasnz.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gpwawkpgf.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gapazihdj.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gcnusyemd.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gzqjjjqhd.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gxdesgqil.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gusbrfbsc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gqgkidumu.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/glwsgdpcd.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gsudcqeyz.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gkhaslmls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gkvitqcaw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gbhkzueyd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/garwdrvxs.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gtpkphgzy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbkphrqxr.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gptqcnggi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gtmmdquiw.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/garmhhuxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gjtntcaxw.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gcrwmpybd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/ggckghaij.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gqfcddciq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gjtifjwhd.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gwgiyexot.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ggwucjely.sHtML


<!-- 参考信息 -->