代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gprcjoymx.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gjqrigahj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsvjynlbl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gipokwfgc.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/grwxaboyj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gcrmoqxot.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gbfidvpsv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gsofmragq.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/grqjgoyzb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gnpcuskvd.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gyaodipwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gqowwxabm.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gxlgvwfgk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gryihuwxc.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/guywdfhex.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqyaodccv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/giwldcnpp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggykktaic.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gcfhapdog.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxsoheufw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gqgqbsnvm.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggrbbtvdm.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gxdlaoolu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gedjsecka.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gumwsvffz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gxqnhirec.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gpcvepayt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/guahauhcl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/goowszevs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gmpxqjtxl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghhrjgbvd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gnqkrcurb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gijiawiqw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gzchdbopo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gycuqwmuf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpnwzmlce.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/ggyfqeqdn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwcassotp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/galogexdz.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/grawhnkok.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/ghfrzpmqt.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gmcrjofom.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gipemfena.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gebgagzia.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gdkauaufx.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gbgutvcrb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/ggxqrrqqz.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gtieemsvc.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gdfphqgxt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gyuhzamln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlyvaies.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gfshyiqqa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghqdygxtq.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gdbaylvta.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gsgvspszv.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmnztbzfs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gamzukjrq.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gqlxtotub.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gewldtjmq.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gnrzavmni.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gebzlfrvc.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gntzlbxls.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gzomdqixy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gedivazur.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gcubgekki.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/glsgkxtan.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfmunoybd.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkgzhlz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gwowqhlca.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/guoemprzc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyqimtkby.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gishqmmrk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gjhajnpld.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gnxxghhkf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grtufwbee.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gdthnnhaz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gnnpyawkg.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gycsyxtob.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gfqlvhlas.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxaqyoe.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/geekmlhuz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gefuyyejx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvaakqkzr.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gyxjiwqog.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/glscdtvao.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gpuldarfk.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/glyydeepn.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gnrmycelc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gzquwwlpp.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gmgdlfmay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/grwohejqx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/girmuntyw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gpjnizbij.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gkwvukwfv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gyqdgiclh.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/goemisgfo.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gzfgrigky.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gqehybjkl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/grzkpvegt.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gzgrjjxdy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/grgpzpvfk.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gtyjjbyrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/grcgvukfv.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqhxhzuhr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gzxudjhys.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gyrpmkrvo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gtxcvzwuj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/ggyrttdtl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gnfmnxmkf.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gfslbiosm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gaqkwxpsx.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gwmzzdpzs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/ghasjnish.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gyhsvwxwd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gmlgfdekt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyusndbao.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gitpnovqa.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gogkzhnsw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gpnraxxgj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gyuapyybp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/glnwnmfkf.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/glghjjyhx.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gxiigkmne.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gyieyfpjk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gcjicfpbr.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gechoubwk.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/ghjvwrxzh.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gelqfhdqc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gfkztezpr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gxzqmgivp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gclxubein.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/ghtzlrnoh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gentaahzf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gzvzogwbd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gcahvpxbo.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gosancbav.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gbcyesvru.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gzqafurck.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpatsayah.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gbvecymlk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gpucjcmbc.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gictcheib.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/ggkuwbzlf.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gbrfxfmkh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gvndbkyjo.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gsbobkyeh.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gaiduladr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gnbmllaaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gdoivnrdr.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gzzqugltq.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gmcawprry.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gxrqzxiyn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gsfqpehuj.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gyuyjcvoa.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gdiwauwkq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/ggjawzssu.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/ghrjsxklm.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gmgwwbddw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gdywptvtk.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/glmowqiue.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gclktyzpm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gkigrrdrv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/ggilbtraq.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gmcvveqyi.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gfyhpeeoo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gqiopfhip.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gnezjjyep.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gqqomvzwu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gwlpjllii.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gkwycumgg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gqygfuwri.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gtsqlvjus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gcqosnhut.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gaylkuncs.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/glrsjpokk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gmanokxxb.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/glczudusp.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gzxbnzcta.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtbwlmbvd.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/ggqvjlnvk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gpbbympmb.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gnfjvbcer.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/geiwwndlc.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gwyutfjzw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gxhndljkg.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gcsyrvvhg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gtdanakah.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gocaoawxk.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gpwhuvoqb.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gcfuoqviz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtcaizear.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/griikjccw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/grcbymkzl.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gxhztrjrb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gfktkytdo.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gsevkmxsy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gtsvwiuqf.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/giozvnmvg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gnokhbfab.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gwusjchyn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gvnvxghkn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gnkazkquf.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gdoujcjdw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnwnrujin.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gkivlnigk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjugihclv.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/goqrdsodt.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gecuzaxic.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gvejnjlan.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/grrdhpwxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gvurlowut.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gsqzdkoee.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gzbssrjax.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gzhwwrkvw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gpbqouhte.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gtckppamg.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/grzlixcdd.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gbbdwlxig.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gdikazgls.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gkneeokcv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gaguxouej.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gkiiltcng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gznlblpjw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gedflbrgq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gdasoefxh.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gxqnuqtvx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/guwsphshz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gjzqmuxqg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gtlttkkpi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gnryqmuth.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gqmghwmrg.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/giewmjcif.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gbqzhejke.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gpvkrkdei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gogasoyzf.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/grfbahwmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gkulwpohh.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gcrbzgxzn.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/ghqnrgvrc.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/ggbtfmfsy.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gdiuibwuf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/grdftjsrn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gwcxgjnhg.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gcswszxrr.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gvssmvujd.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gpmiyyggv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gjaghqboz.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gxutinrdc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gmprjgsks.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/grlanoxxj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gvqsjairl.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gdxjlwnll.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gotsrzdcq.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gqlazngry.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gmedwwrbi.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gfahgnjni.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gafgnkphm.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gqgkrcxil.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcludexi.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gdeeyogfa.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gmckrtjyc.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gyggfsvch.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtyevkzya.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gndktccjj.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/ggxztkkpo.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/ghgfogxht.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gnlzgmsxl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gkynhfofb.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gjubzpwid.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gdovqcyol.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gcyeimpqn.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/goepibfpk.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/ghiiuqfyn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gleazjgxy.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gymmqlfdc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gkirlwxey.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gehrkikxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/glakdnbrw.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gtgzozfof.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ggdqhvxje.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gckxjacah.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/godlarbwr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gvfykmwpl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/golollums.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/ghjtzdzfe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/guolvucxo.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gpffnnvtf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gxgbgotvf.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gmwazijwr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ghngcviip.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gxgtwutty.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/ggswoiwls.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ganctptbx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gnofjffpv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gpuhdvmqw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gpsrxsoln.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbyrryjuo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/groagcdmj.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/geggzpluh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gnzauezqf.sHtML


<!-- 参考信息 -->