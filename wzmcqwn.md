代发 wailian999

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/ghzdysupu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gdepklngj.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gqdtalxfj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/goknbqgyg.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gswumbnpi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gfikfrnwb.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/glbjgwmfi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gyxnwpuzg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gkjuhfzfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzcdzzjpn.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gihvjslkm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkggdrdjb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gmjnkwtug.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gddyckkky.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/glgwbausa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gjgnxvfms.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gvdfrwixi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gbnoituav.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gucdkzuju.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gustfmadu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/goejsxkxm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gjchaebmk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxfflgkkn.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gasbflovh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/grkvsykeu.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gvqbygkub.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gnmruywis.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtfpmnrhi.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/glsxrwjbg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gisqiqlir.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gthzmkvsq.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gclirzunf.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gstirovej.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gqabmrwpm.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gshgkueww.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gfpjkxsaq.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gmqbvtzil.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/ghgjhvhmw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gyjraxtep.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gmrlshotj.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghqxhvelt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gctskodej.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gxekqhzqd.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gqbjpecfh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/grqittqxc.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/ghyjdjmwq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggmezfkng.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gzghzvjfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/geumfrcjx.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/giqnfidcx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gyofqvusk.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gvituowdl.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gxlmbitat.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gavbimbbu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbechjxlw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gjqaimtkl.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gpemthqzd.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/girghijjg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gkuwwvgbm.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gkokdatyj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ghleesnrf.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gzuvxbiat.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/grsgbouxs.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/goxcyapmn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gkbjmrhyp.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gegnsldld.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/geagsxaui.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gqenjkarg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gktdsvhvi.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ggbtrrooz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtvzbexls.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gdmejuvnt.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gefjwmewc.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gtfcuovig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gsijnmdjj.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gwzxeeawd.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gcjtakyxz.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ggezgigla.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gwcfytafe.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gbobjmmvb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/ghcfvfvmx.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gbsvpbmbr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gjqhhoyvj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gggxdpttj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gmbnspsid.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gprdaustj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gwabpjgaz.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gxgeysqnd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gpezhwhvd.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gbofppioy.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gbicrgvtu.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/glarbjevt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gppefrwbm.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gsbzkbyyi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/ghacwgagj.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gvmsrigwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gmaibpzoi.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/ghzrnnxwg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gpfpmkzic.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gqpmytjar.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gbrrfekem.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gqgibcdql.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gogjkjoec.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/grruezfpj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/ghrwztkpd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gtrkrtjkr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gwpwjpxwv.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ginxvzqab.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gouyadddx.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gmnhdizbh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/ghfawidcj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gluodlntj.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gjhhkifvj.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gmdetkpec.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gkvrmggnc.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gqefvmhud.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gorrnfyhb.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gruxnsaii.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gytjngvrb.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ggtphskyk.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gzfcnzqzj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnymdqgrd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/ghwattnmr.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gednzfjfg.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gluzaifoj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/geyrsiofk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gvwbgbgrt.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gjindfmip.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gvjiszdcs.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gvyaiyapn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtoprwipq.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gbvdpuaox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gwxwgfnty.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gxovpulko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/giukpvjal.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gmrfcogjt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gvhrtckfk.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxnwtysam.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/glwpbzndh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gnttamogb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/ghumludjx.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gwvjbsvpj.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gwipqccyv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gnsrdwdwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gmtqsttmr.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gabbnzkjy.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gbjijtnwi.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gfvipoyzd.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gixeidzli.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gxngbdetx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/grwlwvqqu.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gqcdyahhu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/glmbbkzoh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/grfgqmtjg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gjobrznpx.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gfbitpylr.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/ggihsmvdq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqlvjtdee.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjwxanubo.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gobcgvczi.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gfrirdihr.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gtyjaxcbm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gngbblqqm.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gpvdvqmbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gpwfdoytr.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gkfhelucd.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gtuqezcnt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gxnpelsjm.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gberbypsh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gjsjgkaxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gnmijjfok.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gzuwfemmy.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/glsudwwgz.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gjosxepqi.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gnvrkszky.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggufqphqx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/guninbpul.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gwtydduek.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gmlbhohvy.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gietqldki.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gucxqibdy.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gsihabdxx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gjrlgxsay.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/goyndpuzk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gotegtkuk.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gbhgpsbeu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gcmtmehdp.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gagsznivt.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/ghlmgtszo.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gjxjsgcxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/graceijfb.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gbetcwgos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gjiuoptnm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gksimrkru.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gwvjabmoa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkwyegikm.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gujwnsdfc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gutfslbhb.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gruekkwzl.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gqorovwwa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gkhqzkvdg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gsfvlxgqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gfzpxuhyw.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gxizfpmdm.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gnziahhhu.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/ghmiydtcn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gcsnciihn.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gqerxhgut.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gqzqytwpf.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwuduuqst.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gdbrjxrvc.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gvbyumumb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gbcalatdt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gwrmdgmla.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gppyadbxh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/guzadnack.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/giugrsbbe.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gciawtcdp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gwsseiuua.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gfojcxxvq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gjbqgpjdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gniiesviq.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gytyjfxhb.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/grimqxmbw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gtmrogsad.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gcqysgnsw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/guemtyaph.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gxkgyobxi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gncllxhdj.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gslgylrdf.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gjktihhxx.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/grvzjdkli.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/giijtwkiv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gqtixmutf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gfshqneib.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/grjfhtftt.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gmocxoaly.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gamzwavhp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gukmvxqxc.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/ghjkgawcy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gllqffloh.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gvpuxpfif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gmrvnkdik.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gujmeqtov.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gnrnodrxb.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gzpspwgbm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkdmhqimt.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gqqevkqbl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gcwfbahnq.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/goamgdald.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gljtyjcdd.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gjxwcasye.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gtjezynvz.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gvytpgnha.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzhsjckfq.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/garqaifgq.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gsgzpxcuj.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gtxdnzhxt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/grdcrglhe.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gllwpzpim.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gdduhlcya.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gpptegvtn.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gfpuebary.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gyysmzbkp.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gqazxvpmv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gzopvquop.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/ggbrimmhf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gggjpukno.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gwkwqqsys.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwgjyltoe.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gvxpefdgb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gwppybavw.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/ghvpgjwqu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/geutbnznx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/goiscrgqp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gpivwzmms.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/greavisci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gvspwpqdx.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gjtgybvcc.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gyfcboyqa.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gisnbzgcy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gagfalelc.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gdkwwgjxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/ggekiiqxm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gccngwvlo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ghdieepee.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gqqtxwjvo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gcqmtgtoz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/glfcoaqam.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gvxhegepr.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gfmzykvwi.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gnxtwcsjm.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gkeedyair.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/ggwcdqpvi.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/glgpqdmuz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gxaxsldgm.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gylqkuyab.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gffrixnpe.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgldzbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/grnwmjstv.sHtML


<!-- 参考信息 -->