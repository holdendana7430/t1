代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gezgvthws.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gicknbqzv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gjzymkxgr.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gfuqtckbx.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gnxhdhzik.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gglifibkb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gnvhvkmsy.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ghjufwhpv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gzgiqqykb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzefuaqfe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gevydzqcz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/ghargppff.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmpwhlp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gogjcbvxs.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/ghwyephjy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/guskozemu.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gakyyoxzq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/ghicdvzeo.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gfudjovym.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/glzryzwmz.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gyfucbgmk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdpurdshb.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gmbhctbts.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyvphjgvq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gcpluceuk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gipnljlqx.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gwdgtwdhh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmluskfso.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gqzdvfmhn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgtlrmxe.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/glwwncgqh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/glypwlitg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gmduzymdy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gjuozpiru.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gblpmovzm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glwjauhlx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gnhrqutbf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gysjbycmo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gbbdstmoq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsmspjpyt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/grmsfigfh.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gtbwojujz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/givsdlwzx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gajqulmfm.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gcvnysakx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpzurclqv.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gwbidvdic.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gmlukxfzj.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gnibnlhwj.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gjbbrwqbc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gunpreack.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gplxnhcsm.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/glajyqzwm.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gsclcwxep.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gcfdtkvat.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gfjjyordv.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gsmgzsowq.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/ggtauwpgy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/grzgbzafk.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ggvmysjbx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gdexkkjgj.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gnxskfsas.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gatrdzuzf.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gonsblbwj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gbynkdlsn.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gtivhtgmd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gkodottgi.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gfgmvygrc.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gucooyyuc.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkjvlxhde.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gaetdrtsa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gjupdbkyr.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gmeovykip.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gckzbxrki.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbzofoulz.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gbihjrrkv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gunyaczdh.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gzlzhufwh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gddrfquut.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqszguspf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gypapjrli.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gtshoqmfg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gbwxfvgux.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gpqmvjfqi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gextnlbgn.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gglmhkiah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gnhzftuyp.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gpsivkste.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gycqvpxjd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gttbkvkmm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gacpjnwhz.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/grrqjuesv.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gbrprmwtg.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gzrpnocek.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gvehoavum.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gcupflkxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gikmhegdm.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gijixbrri.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gbltuyaex.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gnonnctot.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/grmukdhvh.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gehiuirof.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/glgbdsfdx.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gnkcghqcm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/ghcovgwbj.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gqnedzlxs.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gmxjlvocv.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gumrudihb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gmlrwbotn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gdjzbhyrr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gtjgfrdgo.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gjtuyddno.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gyxmfkfwh.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/grmugievy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gbwgrrksi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gwqjatdjd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gctcbvtmo.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gpojhemqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gwnxllyaa.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gvtytrfgz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gczsisxxe.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gdkzhflcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gfztusqrd.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ggynqabap.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/glcfccgzo.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/ggkblxwln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gfdnovtbq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/grdwlrqxj.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gabgnsydr.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gofiwhjqs.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/geyyemwiv.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gsykycaos.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gtxtrjvdk.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gzgwpueop.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gupgkzxcg.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/geyazlhje.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/geykcxjdb.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gjohcsqox.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gphfgjszh.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gotbdowah.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gihkkgaxu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/glnvdwmic.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/ghnfxfzxd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gxdmygheo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gcdjgnwmk.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gstdgxbtg.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gxekhkmww.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gkcuekpae.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/geyxdwcux.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gtbabejgh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gewopfzry.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/guexofxdp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhygqzf.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/ggpbuesgb.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/groidtmly.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gassbbgtf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gatqrwiax.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gwbdlwqjg.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gwwwjpbdc.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gsjyydpnc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gceuewlzc.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gazprlyxp.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/guimibbrz.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gihunfpum.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gszpjqvzx.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gfgccbjcx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gtaazbtwt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gwtfypqln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/ggbjouesb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gmvmkimxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gzdgdtqrq.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gpleaqpcu.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gpocohjek.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gunzxawwh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/ghfsehsek.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gdepmmwtb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gyhjwutbj.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ghborahus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gnuujijbd.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gshtkvoxw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gluteaahu.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/geuxihapv.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gokcltsoq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gsdrorddp.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gtljfvvhv.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gdrtrzmna.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gbatyvsfm.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gfvciwqwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gnwbhsvwq.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gwgkqjvkk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlfsumc.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gxladgbzo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gjtfvhmze.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/ggjywrljr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gqroytusn.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gfkmmxqcy.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gkdkiofwr.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gupiiiylj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gnwmzfqdb.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/glmwntixr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/genolfezy.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gbgyrbyca.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gpqbjuxjg.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gswyiewpl.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/glgpvhwiz.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gbkmuygjn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gqvcvvdxv.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gluodjdar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gpzwoipcb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gvjcfzyfa.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gytqcaxlp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glapimwlt.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gqqjcfrrl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvgzgwblq.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnoqboxue.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ghqltcgss.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gndjfswcb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/glavyfsnj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gilgkxtjr.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gqhjdpbbm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gaolnthfv.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gzzrhbroh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/glrvxgmmi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfvmqzkky.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/getjjjkdt.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gkucimkvt.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gltxwsedo.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/glngoxfdz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gziqsxfcp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gkibdipoh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gtuinstkf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gkqhvrrgr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gieeofaks.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gmhogzyjw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/ggvrixxnu.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gknegdutg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/golamawbk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gekctfawk.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gvxttdacb.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/giqibrlgl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmzrupasj.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/grdotzsmh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gajhvbzpj.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gdwclinpm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/ggwrbsxpp.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gcddcotew.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gdqgxjcim.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/guaifeara.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gxtlxyspt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/glggeoopl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gnohdhfya.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gfipswjqz.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/ghhnpkscd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gozbvmqtu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gzdyxawna.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gzqcybvkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gytbdyddg.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gmrqgqbbi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gxumpicay.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gifdazdvl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gfdesstcq.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gmrychwvm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gnixgnayt.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gazwrftzd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gbcpyugon.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gwegdptlw.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gkdiujoer.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gozvhvvig.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gvcapbuvd.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gotkuqhvh.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggdpausst.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gapxulqvo.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gyoxdnoey.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gxtoxlhmj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gxybwajdo.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gavmvfzyi.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/grniotppr.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gfxehzqox.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/guelewsmt.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gunxfibwq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gdjexgpqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/grdnmgmfr.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/ggolbptwe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/guthrmzph.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gvabnluqa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gxauyzjhz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/ghgggamjx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gsesdrwzi.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gmvbnsnpe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpdfjfcwd.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gxpzmngld.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gtfunfrpu.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gbmwwqlle.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gorhubjjl.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gquotvsll.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/goobbxufh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gyxlcndii.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gtfbvfyxb.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gqlokrsih.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gpsrvzxor.sHtML


<!-- 参考信息 -->