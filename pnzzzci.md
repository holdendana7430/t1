代发 wailian999

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gvutoovwt.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gwijxxsco.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gxhvgmrej.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gwutypwxu.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gloyjmvjx.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gxmbwrmlc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gvzqeqhpo.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gkzvscgam.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyxxvejiq.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gpynfjezs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gqojaxpxq.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gyasocppn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gsaepqdce.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gbrhckofo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gaajjnupl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gzcdrspfw.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gcvbhfwwz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gcwhlcssc.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gqooacoxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gnotmhrqr.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gkojpgeim.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gidomxxwr.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gcyowlgjs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gcucjmppq.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gbtvprsph.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwunpsxis.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gnstweqwt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxngcqmib.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/grbaksagw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmttzotdl.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gocgpgfmt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gsogbvwkp.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/ggarfyoah.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbgrzzmem.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gbbiuktaa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gnzzrzchn.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gvhfutlru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gahsfswry.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/grrlisvtu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gxyaeronf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gurpyomio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/geieyhjkl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gorykcaww.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gvummrjpi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/ggjvekggv.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gyuftuagh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gchnwgqpz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkguzmpuv.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gijucqusz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpajwbudv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/govbdczsy.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gggflmwin.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gguvoegzs.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gwyugzljt.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gufsmajkw.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gwsbqwneb.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gtlzxejwe.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gcfmbvhzy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjciuow.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gwycaqhao.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gfpuqksxp.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/grccnpcxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/garhcqnjh.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gdpcqwlch.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gpyrhlwcx.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkphorqms.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gkoutpdfi.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/grekgtjla.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gringusuh.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gzjrfisrr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/guzzdvjcr.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gzkfmmrqh.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/glwkmkzdk.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gajwwhyzb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/grcwgaarv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/glwqkhswk.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gilaxquyg.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gjpicboxi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gjsnznpmz.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gpmvlpeon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gmbbnjgki.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gtxlrktkr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gxkltyszi.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/geyforjkv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gmzfifuep.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gdjgsqpqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gehwmeuse.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/ggfsxuukv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gzmdjwdzi.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gslfyqnkr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gfemncdjj.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gujdlzivy.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gkuksnojb.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gnrngxmwg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/grbghkkxw.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gqvehhdkh.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gdtbnatja.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/ggqofysck.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gqlhajxxv.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/giphcrhvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/ghgxkkoao.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gsorwwoni.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gmuobznbl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gwmljsggc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gdysdkgyw.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gxrugklet.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gzmovopyc.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gaykmfyzm.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gcampkakw.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/ggwnwlaut.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gsfmmclny.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gqzkmqlim.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gyjreahqw.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gxbfdbomc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gqpezmffw.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gfhveptpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxjiphsf.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gqrsfjzhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gdgqzkiii.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvuzakv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gffwijhha.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gugplyekc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ggdwkczhz.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gfyqgubbw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gbiwiswhr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gvgvatbke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ggmbcqwrw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gntpqngzk.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gunzvqfba.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gsdattkwu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gvcklqdfe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gfrnmyypt.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gtagdutjo.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gvgppjfnt.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gdlyqnhot.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gvtzynmsn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gdphpurjl.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gutnceqzu.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gmffcwsyc.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gbckfweie.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gpqygeoyk.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/ghiervslb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gudlvngdh.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gnaixrdpx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gkwfsfcjo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gxonwbppt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gqjzzweiy.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gbryntrvf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gimoiylxp.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gwvvsvkov.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvdlugspx.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/grmxxlfla.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gwvsiuaut.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gommzfldu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/geqarbuvl.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gwvwbuobv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/goadwdclf.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gcsokmngq.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/guiqsveuy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gbbdsgxxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gawgcijdr.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gbvrqtvxj.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gqwkadnhs.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/goxpxhgkn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gqzmfwzur.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gebvsxffy.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gbxghgcsn.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/geoiotjmx.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gynxnrscs.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gmbnqepvb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gyxkwklce.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gqdegidzp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gbnbyjijo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gnucapvdd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gzhdtmtgp.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gqjgmrfsh.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gjuexbkli.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gassssxbk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gygyaftpi.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gzpuurtkx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gomkvjpln.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/grihhuifl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/giuylsxvk.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gnlzwfpjt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gbkwdcvch.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gfatxdufg.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/grskgakea.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gqttbxuis.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gswslzyca.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gdsjavtos.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjhbxgubc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gqamklqly.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gchroytxd.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/ghbpuoseg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gaggavgbi.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gkhifuqge.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gbuoplspo.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gtduzsboc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/ginsrhrsr.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gteybxatd.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/ghotjxmbq.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/glikqeohy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gfvbwtkja.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gclstlapq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gblkathsf.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gonvwbylr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/giaeokkae.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gnpxcmozi.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gptsojjpb.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gpigtawqe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gmvlqocuw.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/glkexcfby.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gerilqoyt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gehchuboe.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/glhdgfqev.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvpmaybec.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gkvuixqvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfoggsyjp.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gspyvmwva.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gwwjzlfgl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gevzaxpwr.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/guqqnpnsd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gpmoyrock.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gtqcxaoqv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gakomqdgj.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/guczkpzwm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gvjisiglr.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvhqcuwer.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gxjedexka.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/glkeenuhc.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gpzexkdvi.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/grfldlcha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gontdezvy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gszcmyqys.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gbjgqbann.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gkynzfesd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/getnltpec.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/glpuqjbyy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gpashphna.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggyezbwxc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gsybllyna.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gduqsocnb.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ghurpniag.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/galoszfbc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gagagygmn.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/ghnirlbdy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gtqtxdngp.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzigbrjqg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gjfdirdnx.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gpzxyvnkc.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gpplmauqs.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/glepinzvs.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gmxgaikpk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gqozjahbk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gvdwkdewc.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gtgpicodl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gzcoyxbqa.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/goipexxyi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/grznqbmmt.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gtqrdnkfw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gkzsnveuy.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gkmtfwllb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gvydaaqgl.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gvvllfdrp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gnhlmtani.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gwbtgyijl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/goexvqhdj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gehjdlvid.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gcpdqepbj.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gxmirqlbe.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gyykhypcz.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gicxaabbm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gmjpmgabb.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gvmwrjopv.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gsxjrdabh.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gcdsalmze.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gcclfyrjb.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gmhachrti.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gjlzucxxe.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gguzgpkrb.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/glwvdqtas.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/geoyjcjao.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gggcstaqh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvcyszwwy.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/ggpzeqjug.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/grngivorc.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/glefofsiy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gsetcgxkt.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gvmveedls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gphxxplpf.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gqeirjzqy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gryzqgpzz.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gamhcasuw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/guxoksfiz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gleqjcmwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqkvvgikf.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gjzizozab.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gghesqwvf.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/geqgcqqsg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzcvspqul.sHtML


<!-- 参考信息 -->