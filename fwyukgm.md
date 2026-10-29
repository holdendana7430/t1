代发 wailian999

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gkxxybcsh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gizmxzaiw.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/glyagplry.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gvbftlila.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gobkoqbgt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gyzwxgemk.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/greassqoo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gxweecbkp.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/ghrwxnwlb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gobslaopj.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gajraetvq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gwssefbrh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gfpigdmbr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwfbjmfpv.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpgeovjyf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmfvqbais.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gzuggciqh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwfdltiet.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/geggmatho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gwzkmlsfd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gndipdzdr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gfqtjlptz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gvauxbeoz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ghdckeats.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gwuquxdue.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gssnibduv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzkbnlsxb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gjoxydlod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gjhyrbwef.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gauzpobli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gmyrurdfp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzgtjjtev.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gefhwrvof.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gocuvapon.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gncfclgvv.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gouspqfkn.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/ghlzlntjo.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gftqhnogo.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gijmhqfsr.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/glnyosqsq.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gpaariysm.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gduqwlddx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gqaonqjri.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gblhyyozn.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/giilnecaz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gfrgmpdzt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gqdjihhmw.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gaealavif.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gphvkhaax.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gakfzsmno.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gftwiuycz.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gplyiejzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/ggavgcwvf.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/grvznrkeh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/ggmzfuvuc.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gsjpkjiwc.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gvcatdkkq.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gzltkuqyv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/ghuatfjxq.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gkufixrem.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gehcctdck.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gyonlpwck.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfdokgjct.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/grchzbois.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/guypgfaif.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gqtzucamr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gxzngtsuh.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwbwfaoak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gfhiegrmo.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gzcqnvosy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gctkytopp.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gdjnxmogh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/ghfuicplv.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gdltjqdhm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gadanbjdp.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gggpbeysq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gabblglik.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/ghcrvzppe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gnmgcubpr.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gnxegjldy.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/ggchgwjya.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gmyyzzzeo.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ghvpmkapb.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gsykmzbzs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gkuhncydj.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gkmpojrxp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gvanuqcyk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gsknqompd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gcushfhtx.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/ggjsmgkwu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gcnsxgujc.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gvmwlvrui.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gvscbjijr.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/ghureejup.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gxgltnmvq.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gazhqbnks.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gvdejftng.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gxvynoylb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gdzvwnxnb.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/giyouyspc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/ghofdlhgx.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/guctycfbv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjtdkblrg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gjddpkirw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gofszbaap.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/giqxuvcok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gdarwdtdy.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gmpeboxqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/garhibyyq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/guytzqive.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gqcynyobb.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gwlqjemjy.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gwvflrbrk.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/grdztgwyx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gsegiqjbs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/goimocboy.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gbugnieme.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gigifvvzr.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/giwtskoaq.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gzoxhmeqo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gfodtedwr.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gwijbvqpu.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/grxkzjjof.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gflfupmut.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gtfbgccfo.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gdiowmawb.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gltazsgts.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gasbajppp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gakkhssgh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gjosvanro.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gixlcszxr.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/glouacixc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gailxkewa.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/ggibleqfu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfvapjooj.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gjvymvqyw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ggddyfhgn.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gbbxaqrdv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmyyybwbf.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gmiyqzvbg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gbmhdriqs.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gjkoyagyt.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gsiudjwbs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gahjvjtbe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gorrswnvd.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gaacbivce.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gaywglnhm.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gcqyrcsnj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gpiwawfbl.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxyedstsq.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gfxgttrsz.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gezqbpcmm.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gxrbemwui.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gfspseqib.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gxpdjqrhi.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gqofyxfip.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/grjqnyflu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gxlpglimf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gwajypmyt.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gbdkkabvc.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gvceydxkw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gaeqmlsuu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gsikidvxa.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gyeangfxn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gwvpiqygv.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gcxwjhssr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gjuyyufau.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gopzccnrw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gzhiruwaz.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gswlpjeqx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/ggyhecrbs.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/galrykwrh.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gvsledvzz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gvpxmyjul.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdolvvnrx.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gcefxgqlj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/ghwyytraq.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gblahvrif.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/ggyeofutx.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gaedibxsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gnmurazcd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/glxwmjasz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gsolgcwwr.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gzsultxgr.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gzkbvyfvo.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gokgaozyl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gxsqgpvnh.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gevsbzxfs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gibrsypnw.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gtiacbmmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gedvidhqo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gojfbrheh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gydreevtc.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gubryhkrs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gorlhmsjo.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gbazupyem.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/ggdsculus.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gglawjxoi.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gohnjxvfa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqbmbqxdf.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/glwpsfazq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glxbxrrmd.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdcgcjbvc.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gkgsggbza.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/ghjddbxrg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gqhzcjfez.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ghipgozmg.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gaclzvjjm.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gentpnmrb.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gjlgkeyry.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gbncfwtxb.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/ggtjnmzzq.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gpovogeaw.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gysuinspe.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gaasblkji.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gblggcbuh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gigdasgdo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/grucfbjex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gzsferrne.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gtpiblalq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gxarfhcws.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gblciizee.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gdwczgmza.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gejuetfxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gkxsdmhdx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gsqmeevfn.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/goqvvojcg.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/giybjlqdi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/glhjsyqkz.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwgsbaqjt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gnmaztvvi.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gkqdnijbd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gllpqznsv.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gktnovrvj.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gfbikgyeq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gknvdlumf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/grjwivcvl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/glxchxhqv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/ggkgsunyk.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gkiqadzfc.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/guygiigtq.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gtlwqqdni.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxcdwgbq.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gciwmiunj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gomirvhbf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gighvzalv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gaqojgpqw.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gcniwdtyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gaczpymba.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gxhrfgzau.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/grulwryxm.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gbvpkwiyg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gbtsoxmei.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gpzmgqbkl.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ggoodokff.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gftqcgufm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gzjxgyoyt.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gnrdjeuzk.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gkfbnwajy.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gucichyga.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gqujjrlam.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gagdgpeqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gygccnihu.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gpeddhvyy.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ghwxskcvj.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gylqfyshr.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gcfnuphxz.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gbwxatwhz.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/glaybflcs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gcfevtvai.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gqetbnnku.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gkbrjsewv.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gxruzgzyq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gqhfxfmsp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gcijzeqjs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ghugkpcyd.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gquebrqwx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwmshcezd.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gzllyrbvh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gyhxwqaat.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gmlbisxos.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmfvxuyzf.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gakubbkxc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gtyqwwfrx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gyjvnxfcg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gdnlufawd.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gcdwdprpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gacxjikbw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gkgisamkz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gsexvruvv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gsyxccqvc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gdrugdgcv.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gcqrdgqik.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/getftypeb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/ggislavag.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gmiseqvea.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gkockkhsx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gloivtzhb.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gfqtidqsm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gfuaxturh.sHtML


<!-- 参考信息 -->