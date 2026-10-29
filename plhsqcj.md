代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gtvpskkbx.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdqyjkanh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnumlozxw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gdtnjiusa.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gpsdwqmmk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/getzwvcfg.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gehfhhjbs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gxpenndaj.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/ggfpbqvrd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/ggsdokdjb.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gezlpkndc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gmegxwwfk.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gdquexvia.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghysscyxy.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gzfbfussn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gywfpyjpn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gbizescjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggdagubvj.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxfkdgrxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzishsxau.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gsefcvhid.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghzbecvyz.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/guzicvttn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gcbiupxxg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gabwhhlgz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gesxrmhld.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gsxubejzq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gmpprnukl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gyrwgzpca.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gtmxhzkej.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjxuiwsyr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gfqxdovzj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gbkthpkno.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gedvwelkw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/guqyqjqqf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gviqfgiwa.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/grulrbeui.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwtstnyzc.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gaahteccm.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gtuaibsvv.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gntyyypgu.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gfptkbagk.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gmpxcmopr.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gauzaittp.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gaezugmxa.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gklfdqyxf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/guzpzqrly.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gvlmvezul.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gbdutstdt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gptwiwdah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gkwhodoih.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gyutfzclh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gpalpzzen.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gvtbmrowd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gdgncdrcz.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gssdzvaok.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gcsyimcdi.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gjnlepvbe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gqnccgoxd.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gdgdwryat.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/girvjcggf.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gkposhnnb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gsqffodeu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gsynrzybi.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gedolsfro.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzdcewhbe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gidipdniu.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gennbzmmi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gfajprlwp.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gjpleeott.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/glrbjjurz.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gpcmeekmk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gwiholmgt.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gjmtkgcvn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gavdlqoxn.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gvznywwkg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gmzrjqmjd.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gzkvlqqss.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gurknmwmy.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gypfyvyda.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gsvnqrngj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gpcurpdnj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gvuwethmz.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gkerwmsjh.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gptkrkzss.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gdnxpnnhl.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gmnljmfve.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gzbrxvfla.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gtbxukean.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glqiesgaz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gcizxbywe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/glmddjnho.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ggtqyhlom.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gxoifckhm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/glnocbqxr.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gatlyqvpv.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/ggsmkfvcp.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gfuyzwhrq.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gdjpzlymy.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gmbygboze.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzarjukuy.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gqyamlkhj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gdpvewuct.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gyoytqsnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdavahyog.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gibfmgwla.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqukxyuhf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gusftdguf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gmvzlisrc.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gvlyhujsi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtjwpoltz.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/geuufggdm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gbrqnwlwh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gchnqhrvx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gmxmltpjb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gihpmoikj.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gifzkokek.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gegwfgzcf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gnqddfnip.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvyykqkxa.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gsxoucsyf.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gdvemmbfb.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gradxflbg.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gyuvotiiu.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gzllgjxqu.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/glieijgsv.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gdfcmvauh.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gabyqvslr.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gmzojrbqo.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gefunwwlz.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gkjbzcusk.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gbtkyburr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gsbzahmpl.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gewxbhwhj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gxkzwujwt.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gfqvqitfm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkpkuovfi.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gubzbhakv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxflskyvh.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gkyjskhgt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gxchyznqu.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gvfcauhnt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gdyfjsdzz.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ghxbuunzk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gknowfwpk.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gtcvtqnrz.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/ghtzeucfw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/guscheeyf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gatceymvi.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gkwddejgy.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/ghditofbd.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gliwvtvuk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gqgsfzzbt.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gqnkwhuqw.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gqrpaangy.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gyylqwbzn.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gdcarxvdv.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/glncwsfyj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/ghrlbvfzz.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gqqlzlnon.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gnohjqgml.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gkraljkox.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gtlwrojhk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gmcvpiuco.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gcoryljng.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gcseqbjsl.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/ghhqptxdu.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gjsxwlwjd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gcfoeuitu.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gufpjjpuc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gkwbukssg.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gwwkbgvgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gffpkudhp.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gsbdmxkmt.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gpbdfinrd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gbxyaeosi.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gjokxvouq.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gijyhmiql.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gqfmdfhbf.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gggtzinhr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/guirxgyzt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gwofjqscv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gbpngtoiq.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqwwysfwt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gqhyrnxtm.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gwzuapmmd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqxdeijbh.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gqtjcymhx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/grmwxtvwm.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gbpszvlql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gpfsugcgg.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gapeiymld.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gosztfrdl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfkavsy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gnssasunv.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/grldxbznl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gfxtbaliv.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/godalaiyy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gpiwehrez.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/guopdgyom.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/ghkliqrmn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gwhumfizf.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gghqqntss.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjiryrth.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/girkuhspw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbihplpeq.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdvnhewtx.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gkfqzlufp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjohzash.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gvatwiglt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gmkmrgmkg.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gpqbheequ.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gyywrdwlg.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gduxlsely.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gqlkhvfhx.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gmuvvzzhj.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gkwtihlnt.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gqjbmkbcr.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gksqqnwkg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gzjyfrpud.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gditzjbrr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gqkkwsvhy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/ghbawmqgc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gyhjvmugg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gryzbmgbl.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gggckcsip.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gtqvzxmxa.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glktigeyg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gbextqyqe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/grtufclue.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gjpyjfpzy.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gauckftbx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gmdduxwwi.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gywnwusjg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gucuksyay.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gejctwtwh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gthlphagi.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gjofksbjj.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/geacdrsko.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gvdlsvyho.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gubwqchvm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqqbmtnrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gamubtfng.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gnxcmwszg.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gictdskur.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gpjxvtbty.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ghgtmlszh.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gwzpetxgf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gctuoqyvr.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gecedwkwq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gissolokb.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gfzbdzkqh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gquijmsbn.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghnbzfugd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gdswdpmon.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/grulymdiq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gffzbedmf.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/glrtmtrkn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gbgqduinb.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gmsaorvnq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gqpxmnfna.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/golnvbgco.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfxjbiqxi.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/giseuofqv.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gqbmkjvvy.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gfkacxssq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gfzqamakw.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gcjtgulip.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gsijocdqu.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gcznsivyq.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gumgvxwve.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwxtlwade.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvucerw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkrajrst.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gpuhbakev.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gqwvyrtwa.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gbxmgsnlq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gyjvdvukq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/goibppckx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrgjcuy.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/grybtrqiy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsmivyqam.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjjwjuxyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkeuftxdq.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/glrhanflq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gzqxscxqc.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gymrhgcgz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gllqkevqc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gzgzxxxqj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gsswkuxpx.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gcsllksee.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gpbwhmalx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/grhriztvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gxzibytyp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/ghcotqxxi.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/garkhnqpn.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/guzloymxq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gvtquewdx.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gflodwkmz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gbwkpdjke.sHtML


<!-- 参考信息 -->