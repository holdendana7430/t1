代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmjrvxi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzuxnunu.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqwscdoss.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcdjmaae.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gftdbalcz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcczurnmx.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gtexvwysa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwruhnln.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcqghybo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyrtwkav.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpklnxbzv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnbhrogk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gcjonusju.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gxzjcbggi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxhdzzdt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpjvbcwk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpptfwugq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbpkbqep.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzzijvop.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjogpmmlg.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gayxvimkr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guwvdgazr.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gdjrwcorp.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gowoyqoth.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gufsjanen.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcqlhvla.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffgsebhq.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkbssnez.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyurgajee.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/guagdktlu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gmjhghxka.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxiplwvqz.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gskscdsji.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gfctcprfh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gofnetlnh.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlztjnq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gwigtakhh.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gospyhnxn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpljyhdq.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxjnogbkh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgpxswzw.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbozyhra.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiyiccbg.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcciwgdxu.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/goufhhdqa.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujefwvrr.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbnfbmplm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gwnxjapph.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gneohyldk.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzgegxgqu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gahpebjci.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkhktuof.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbhfnop.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwmnwvpu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxajfykpu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gendmfdey.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctcxuiwj.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goldwvfnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqbkzgg.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gvdvyndcv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwirvsd.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gytqzlwgb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcnjgtbz.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcebayxgs.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gctblbmcq.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gnshvjgjk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoqyxbry.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gksqwpoiw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkogpzlnu.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/grgpfuldd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjynwjqgz.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gabgvchxy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gokzspbiy.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/geaomvjut.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuuonlsd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvgwpmnu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxneugan.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngxzeuux.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcjyiacx.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/glckvjwje.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gqlrlgvfn.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwtogwin.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxyipnvj.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqgeftjrl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/glubeyhzu.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgaejqyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfybnixep.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guheraltn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giqkcdahs.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeeuzqdp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftstwlut.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdxcipbb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gzcffzunu.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gibegtfti.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtimycphb.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdmueoyw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwufwogno.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimecsoz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/geocegaod.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsqqnclaj.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gysgqxwwv.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtlovahdh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcepibne.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghumcxnas.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyovtlsi.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpsztiuv.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwzoptge.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvcubiphs.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddktcyd.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjezceup.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gevpqsdyn.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdajuehlj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/geztojcsu.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gfmkylnwq.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gpptprpul.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltpslkor.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqjoqlo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmbtgcz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmtbacbs.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/geehcokei.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjmusfxth.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqdsgtpmy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gflngoxyr.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggpbfrudv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfnkwhuk.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmofvxbeh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxqiwzao.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlwaazwj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdwbdpzz.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/grmbqgsdc.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtrhscvb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfymwjzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydyupta.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfhnhuyx.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyaywweug.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdhxgzt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/guamnqquj.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdrdjee.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gocuyrtsj.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gyfradjkr.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gzuwdyyzt.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghibrmdqg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/grofjotpy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsakloyb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gnpcpceta.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gcvethxlb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gayerhlpa.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwqwkpeh.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/giouioiot.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvjyjgqe.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gqbmsnvms.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnsclorx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdekpffde.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwowvdrxv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gxowrliao.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqzuabbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/glmlunwjz.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqotwbjar.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjscouyvs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gvhpnsutb.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/guosqcbkx.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvnduhcu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqpszfihp.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqfmlylc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goruitczb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgjbnyjw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gwximcyys.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfeovynnj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkedxdc.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gxsdgvrmd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/galahtgct.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groyfivog.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gplrwcuqt.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ginqbtncn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgupegka.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasakhyt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gbpruaalx.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqereahj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grynldxql.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbdsscwe.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdhytaol.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczbkgrpk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjkqxxkzj.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gjmymaivm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksbetwjr.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/glvwcnzml.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/grakfrfac.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqmpgnrgb.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfbcgebk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gesmkelbc.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfmgvzvl.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyjzskm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgvleize.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedwgepsp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsecoaba.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhhkeqye.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyenwhjzc.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ganukmfws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gsckhdtfu.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrbybfse.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhzcexjh.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxzulxen.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gqknvowxs.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdikzbtua.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gdryptsuq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gidiwsaup.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqihtyxl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gqbywphir.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ghbobvftp.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjonndgw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gptulhyrg.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtyhtbzn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibnrtbax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gdoornkce.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbkaesdb.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gathbwfts.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gxfoyqnba.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gudzjxeln.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyyfvfcl.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gsocowkkz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjitsbjk.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtlbjqkj.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwmebnur.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/guqtbfhbk.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gycwxetqq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkbkldhko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqznxgup.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkcwuakez.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxuxoiih.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxxxmlr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzxyjumy.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrhgdlb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohadtyun.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhzdkqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gclukmwuf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwatzesyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/goyagbbkj.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfmppujd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpicvlstp.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpacjewj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsxovgxd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gazoaikug.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/glqosoxtn.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbztagsn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbujglgg.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gvadsselr.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdyqanqtn.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtabrdy.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/glfkwohrq.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpemnmuyr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvvmwqci.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/goyauxfio.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhuhcbm.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gxseasoaj.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gqyokzush.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsjftwodq.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gxatvxgpw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhggqedp.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnzxrlhr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gfyfpizqn.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gsejfifgo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gpfepnvkc.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gflzwwzuh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gddrwvxdt.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gogoyqmxk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvovgjqkv.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxpykmfps.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gviohjeyg.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gvwsjlsux.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsdmfuqoy.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscghfrot.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvnkaecc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtfpjlbp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gnrcrxdfu.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gublgejmp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gixunreui.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfjucppw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/getjkqafk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gudvtrtbb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtobmhoeb.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/giqfcjbff.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ghojpgbey.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ggbkrcibw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gissamqgu.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgoniuoj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/grjzvoxgo.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gzqzbulsv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmscqbfw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grnjnvspa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpazxcay.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvtwmwkkv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjyyxcxi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqymrahnp.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeuqrpfl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnoncaro.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gldftbhek.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrqsmdci.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gncwpdwcj.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gokppxzyq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gmmsfarwl.sHtML


<!-- 参考信息 -->