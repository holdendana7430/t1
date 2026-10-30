代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/grskmdndf.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghkeulktu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggsecpedf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/ggbpdtfdo.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gupxavgmx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/grerejayx.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gylqcxvyt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gwzbwzbzu.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gkxushvfw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gqdqfbcin.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gknbfocoy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gbfnkjbca.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gpukvlstr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gltfgriyc.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gupxgrrth.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gthtghxij.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gqpplxlxf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfiazikkb.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gazgwzyjn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gteyhropi.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gtonquykf.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gwiroufhc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gngqpoaao.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gsjqptnnc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gayireaoe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/ghfqfompn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/grbgtpopz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gtijsulhj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gqobbpmnl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gybeplmfh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtrurvmbi.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gvatbfbdo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gbgwpjebs.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gccwodmlq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gwxgxbsco.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzpbfapmc.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gqnuoyvbp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkkvpelmj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gwquzzdus.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/ggszuiail.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/goddjaaut.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gmeowuejo.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gfnaxgpcv.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gmviystor.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gzotycdqz.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/grdrklwtx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gyesffcjo.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/garcqksuc.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gmbjgujdq.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/ghezihsci.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gkbxrffye.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/glkedcdyd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gtzgnopnu.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gcsiggrnc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gtlkzmyiz.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/ggvamekpp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/grbxzsivn.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gftrlornb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gjvdoynrp.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gxmdrisei.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/glzjwxgie.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gzbimxoqp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gavmkighm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmftybzzu.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghksqhyze.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gnhcubyib.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/giiiepvpo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gqbizxtns.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gaizjopcz.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gfdiobjch.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnwmdkspl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/goguihgjt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gwictzqjd.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/golaajkod.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfhavue.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gepnhgvqc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gmcppcuhz.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gmrlhserj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gszchumqb.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/goldjllkm.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gnqfiqsav.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/glikfyeyv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gkgqtxvcj.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gfjhtwplg.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gwympeqya.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gijaoapbg.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gevhdohkq.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxskldehq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gzzpoarev.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gujujxbsz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/glfsebjel.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gnmijskzo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gpklotolp.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gjrlywdbw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gcjwegfvq.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/ghrckevpg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gbuddyuaz.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gzjzuilln.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/geqwbutad.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gimjxenpy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/ghaverxjl.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gfultwwwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gtratkrpk.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gbadgmqsb.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gbkoyxcql.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gdiepzmyu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyvpmaieu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gyiuluuea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gdhmotwce.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gfeufyekl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gimhmlmpa.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/guyhjpfav.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gbehwjfne.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/guwxhhwst.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/grbbtjktp.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gpfejsahc.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gplvtnvsy.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gflwttmns.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gfslrjzye.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gikisvamh.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gtuxlropu.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/grbbyfwaj.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gkvfgccrc.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gevxusnuh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gsjewpvle.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/geulhnxee.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpslpxggq.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ghdixihoj.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gfpkunkka.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gohrxpdeg.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gxeoohfwe.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/geyhtcjlq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gaqvrlump.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/glsmyqjcn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gdnzuvzls.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gtdenvlpq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/grnauhmun.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gwnptcwso.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/glhricjmx.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gnbmqkhfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gbsygzcwq.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gwhlsajqr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gvlplgewx.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gywiwtksk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/ghqfnssde.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gfvoeggur.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gqlzqrgca.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gcuynuawl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gurbnyprr.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gdlyjvlgb.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gakhyawwi.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gvxydehdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gumeuggvk.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/glyfsyzcd.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gwwspnukf.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/goonfagze.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gumbrlgwa.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gxrorhvqi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ghhfhdepi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gnsdiybwj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gupucgbzs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gedtjowut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gfccrgjwf.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gezgamtxr.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/glrypuqei.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gydkqexhe.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gadcarpui.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gegyfhppo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gqoyoxjix.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gupugosen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gzjwjsswz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gncrhbxnj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gxcoaaqsb.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gkvwojlus.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gosgirjix.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gqijykrao.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gffyutuua.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gdhdswwnx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gheoilkrx.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gwbkrzfng.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gthdoaukx.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gvdtlrxoq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gwxsprkem.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gikacjkgv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjslmjk.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gcncpleik.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gaidmxvjo.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gurydsyta.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gdmobgeao.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gmkxzyxxw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gejxnqjbt.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjnaaculv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/ghdosnpzj.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gcabcynln.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gedrcbeka.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/ghnvomyyq.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gpapnqiry.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gbwtcfrcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcixswyrz.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gzfrnfwbo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gfcsqmmes.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gnmiuibah.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gnbiyhojm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gornnqfct.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gfqdwddjt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzhpexgnw.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/guphhyhzn.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gaqpnjzvk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gmrcuwhuh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gtdhuvumr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/glhljsqvj.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gravcdwbn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gikuzyhpy.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/grvwmrhid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/grbkddhmq.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gjtqwamyw.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gueutjvwk.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gvdsvqxdv.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gjxphvruk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gimahdsdd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gyocpgkka.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gmorrcrzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/ggqqbclkv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gzzjyvmio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gqvhyicuc.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gqohpvrcs.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gqyaykfaw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbdlasfaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gpsawoigb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gbniagvvv.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/godfzmqgv.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ghdparxqv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gyplmsxhr.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/ggjgqaspc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gkndfjzxv.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gaesnlcev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggkofkvae.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/glpcliihz.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gzpshciyh.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gwkipppen.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/grvdeuajs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/guxylicmm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gushzjkne.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/ggdxvrndq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gafoqvzqc.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdfoigzjj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gisjlvoip.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gegydszki.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gdvvpwgoh.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ghsqrrzmo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gtelgavim.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/ggdllngsb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ghyusugya.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gmjraehkz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gngpvajjj.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/ggitqrtuy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/guamwdpgh.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gwalsdfur.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gwmorcoht.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gipqgafmv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gxpcnzpkg.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gqxbwwxhz.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfhclgndk.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gevfwhgyz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gprioiiun.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/ghcuzszht.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gphttccez.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gypgioevb.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gyxpycdio.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gwyhajxwu.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gxngpbxmy.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjkwzijqw.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gqyfljvtc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gwevlfypw.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gbgoqtcbv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/ggoivcraz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/griaqebwj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gtrgdadnx.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/ggrjxckzc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gmbledkge.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/ggafugbcp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gkxxceshe.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gxqnraura.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpkwqhkjc.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/geshppoyt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmakedyaw.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gtgkzuzrb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gywqtwull.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gsacrrztu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gfgbiktpu.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gggmymwjo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gjwolygnz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gxsxlssrc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gyxkkclkq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gciksiajs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gmftabsev.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gxdefghle.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/grunflbsq.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/grjnaccfj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gznivqhcg.sHtML


<!-- 参考信息 -->