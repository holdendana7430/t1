代发 wailian999

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgdgrlld.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzropnik.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxeodjhbl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcnptans.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtzpzgbhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdsfwsen.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjietchp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gklvygfqj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/ghriyupag.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggnvbfwsf.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gihaxnjqh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/grklgttll.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkfxkynq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbgwvtgi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbpykzhns.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcrgvkcb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gckyrozvx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gatchhjsx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvzfcfew.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gdnyuherw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gctuoxqsa.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gycadqkwf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/geggyaalg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gockyjkct.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzmgsama.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkljeocf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gemeldacn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqulxlax.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghahmvixh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/grmkqfnmn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtnckddz.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpqturhxg.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqphxwz.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gytugsprk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gakgocurb.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbmijfy.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxattyxh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gyghgujag.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmopbywcq.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmppbgtaz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdxqnuwz.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyibjnbp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaravvst.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaeovldn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gubfgnjoo.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/glqkyvrta.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ggmhwxfey.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gymncooym.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gzmcsxrsz.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gejuuxakh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gortmqjre.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gylismtmx.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgeyidmo.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggwsdbjjv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gclogwibo.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaiycvka.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqhpkecpn.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttbofmol.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqaukxixa.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grkrdnfxr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmpnmfyib.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glxiztnuq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gciqixnnm.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gztmmpkkm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvseyvhqg.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxfiqofei.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvkwnurqs.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlebdmps.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gevsfbqth.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/glhmbjkla.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gopkbwsxv.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfntmqkf.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gajfampny.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gjdjqnmzr.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grllbicqk.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhybcunq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gellmtocg.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxddtfuen.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjnbnlnxs.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gcfyaknlz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gofikymnj.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghysgyqed.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypkzlrxj.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrnoucbu.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/giyeijknh.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gjhcdylvu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/ghbngwmku.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqglqeogd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/guwadmjob.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzucbjgoa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsehyxdnu.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiidudlx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqwjwuje.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtianmcmq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxlzjhmk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gicjefwzt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaocnqvmb.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkxsvvrp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/glphagkrq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/grfmnpagy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaudqqbqu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvsrflrk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmdljyrf.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gssgtbwsf.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvfymfwii.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/guowfzimb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqczkbpdb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthngyolo.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprstvmnz.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gljedejwv.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvhhhiiy.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gckcklxcr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/guwtwqfcz.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/ggkekfhzp.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gslafquub.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gupteginf.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grdjvflaa.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gvcjmxhii.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjabyvypy.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcsxsyez.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/ginxhqmhw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gdpdipqsw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gwswsolbu.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcslkjsw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmgrswols.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gneurbbov.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiytkfdf.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmyxtdtcn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcbokkzk.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjhkrudt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggnhablmn.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmthclhb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbmuzkne.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/grdjuhrbn.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypvjmghh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gssinfput.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/giifrdezr.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgtqmgho.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gknxnmzqj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gzqkhruon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gavxmctne.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/getrvtmgi.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotpcuejn.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gumzpcacv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbklxkjdp.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwunwbeq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gggilgqse.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gbikbltqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsnbljtj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guaklaktz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyzmnkjy.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrscwncj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtycmufni.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gugwmwmyj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuilrbq.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxggmyfzd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaprimmab.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjndfwej.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/grvrvzemn.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gcxzvsbkq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/giyqucwab.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gonajqgsq.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmigxely.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdfsasfv.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gorevmgtz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/grxjrrekm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvexdpvo.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gvkksqxpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gpeaqjpwv.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gejitrrbb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnmtisms.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzivwxoel.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqglnuka.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gdeccrvuj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwiqcsxa.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmlgsdqkc.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gxwkygxlv.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/glooojeoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawjmpxbh.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcymueras.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxnmfewz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspncucwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gfheaaexd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gzoggevci.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfxseruk.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gnveyswan.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/grjeikzvi.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gimgnnovv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gunyqxdtd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gupmhftaj.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqxdbcsf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/goeqgiwhx.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwtkobhm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfadvpmq.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobwtygav.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gbyalttoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocgmsrko.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjpystixt.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwuebloke.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjxtfvxme.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbsgplgs.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gkogmqnsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoxfsnda.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gyujdaqch.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjpeilzn.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemokysdm.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gonycnkka.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjchqikoz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpcjqvdr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/grezctqct.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gzwujkwth.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuepflvd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwxlhsnu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gwbkitzqf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniyvlljq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyvytydj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gzzzhmgkp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gjwoizmbq.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksqazoaf.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmrhaksz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrpbhgzn.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gkahsyveq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gnqxardaz.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqmsydbkl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwenzcdcf.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guppepvax.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gjyhodous.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gkykcnmqx.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmbgfdzn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/govoyjmcu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gammbtrpg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrgpeis.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/glhbxmayo.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghadsdvym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqgyrfl.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/glyvkfpjc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gypxqujmj.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gfayipfdi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzzmpmg.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gylkfojrq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzfvvuzh.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gjbbvgkcx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtwoignoa.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzutfuvpq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gzrpgbieb.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcaanqif.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnicdxulu.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifsqkuk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdtqozld.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhaziooh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqevxoyc.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccsogkv.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwcvfyo.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwrhswwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfbyfwoz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntgvgolm.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcszqemeu.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaglsuct.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gitmavxqa.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvqnzidy.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gbnykkzph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdyodvlh.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpttfunwu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmqghobjl.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gyliazqxh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcduyoz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoyklysi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtyljtrqn.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gmshvzikw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwtojoiyu.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gggbtfnbm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/giljeqbry.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsnxpsov.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpsrlzvk.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmayvtwap.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glfabnpxg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoqdwzod.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gnpqvbnoe.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/giruosrze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghaeinnpp.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/geeuxyrif.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyjznstka.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gatravrbk.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gnmnvopbt.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfyuffww.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjszueam.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcloehhh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptiuafdp.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwizonnx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gondewapl.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gxixkutip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvbrtrfl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gemckxpdm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gevimzymf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goqhzugni.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmbvzycx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gejyojnlo.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxazkjp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/glkkwjxwa.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gpogietnx.sHtML


<!-- 参考信息 -->