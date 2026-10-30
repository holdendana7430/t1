代发 wailian999

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gzthermjn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gvmjwyrli.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgltdaom.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/grshhojqq.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmpfctdh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geusmztkr.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfudpghpf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbzjvgkv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmkvgialv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaukstkq.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gctpvtsmy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxivfuiho.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyfjhvry.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaappauf.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzjymtxb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxbdwgsy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxymejpzy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwckmoez.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcdntxmi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gcmuldogl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyevzwcvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gslekxfkv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnljnjhow.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ggrvhhkfx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gobbbcpmc.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxsmgmk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpooevhib.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmlzocsc.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotnzgos.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwmjalud.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gdqplrjbf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmojmiss.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtvzapjw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvnhbnn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvkolwic.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlanlyhc.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gofzwmmpk.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcybiopna.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufzydijy.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gipwimlfs.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhydtlns.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfagkdeve.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grszdwqup.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmlwdcmjt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gitcvdfob.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqecymzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnrqpgkf.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzknvdyt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gltsckinm.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gskfozfjl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghpbyubih.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gmdeenrsf.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqviipe.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvubvoyvy.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/goktmujmg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqyqdprt.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrvglwab.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvuyqclo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxggkqfov.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gysmgukgz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gctvrjjox.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gfkhrwlcy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphpbxie.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaawfywiy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtieqxw.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gktkfafbd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekgcqaao.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrzmbckb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/goeuetacu.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaxkayaq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhrcfpwn.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdcnrvrqj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldavwgih.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnqvslrj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjjajlml.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhgurkmu.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfultdhw.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyqnoktc.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtupqqnob.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjlnvixz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtbpmpka.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkijowvk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyepmcxey.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgyimbxf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gehlmmbgk.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyfbbcecl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gubkplcne.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsjbmale.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grjvleykx.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgijbnwl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfjnpxkv.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaonikhrv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghioivxtv.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbexevqdl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gvbybqzcb.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrsvnucr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmkoytsno.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gampgthps.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrpniuqe.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gceofzyur.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gqopvxstb.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfnblbxz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gkadriiwf.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/grffbcyfy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaskfdqxf.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gsvmdthzf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gwlbzvpek.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsvdygbvz.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvvxaetie.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gsrpncmua.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsbnrxgy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gnnqfrmtc.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpydruwti.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gawcxbpav.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gisslueam.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhpfakyb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpssznodd.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gofbckzcr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojebtims.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gflljcpmk.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/glcmiqpmb.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gofnnjnte.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpfslkp.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztbwzlxp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/geegxuskz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpgaumco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/govhpijex.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkeddztkz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gudwiuazx.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/govjdiozn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhbwpgfz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groxenzfr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gobislokh.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbedlchhi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdexmlk.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gsvsxggfj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gacmomkgd.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gblhypnxr.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaagxtzb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gbcgpqabr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnsmrzug.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfojbmqpy.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdwtzfslk.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gaasnlpjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gscnopfsi.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhzhjqqt.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gkthvzlsn.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gwopectdc.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gmfrtdynj.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtyyoqjth.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrhczqwt.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gmftigvuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gpbvbyizv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gfkmwwigj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gomgzjwfg.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdetzsut.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbtraqum.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gealvsubp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/glcchqhqq.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcymeibqa.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/geevignpy.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gzcftoecd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvdkzuyl.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbboqwix.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/guvkksxnb.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gimesvdoa.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrnbjxbw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrnuygbp.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gdevorblu.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/guqbxwoek.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgwxkvg.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzkzesaa.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/guyvilqpi.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gxifwfpeo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gcauuzqlf.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gazxhbssv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseypczqh.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gjcublptv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grgillaht.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzpapbidm.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/grtzkeslg.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyzvtlyf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/geasstxdq.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/girmtyrpe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqnnzze.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrspaxy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gxskqshmi.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuymnasb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbpfxajh.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpgmufss.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwqzgpluk.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsmdqjqi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeutwowy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbvpkioo.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnvzfykq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpxogcta.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gowcvjqpk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsojquong.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtzsowydh.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gvkyrdpdh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmdnfemn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gxrwxkfmh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gejwrkhff.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gegzqspzn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpesoekhf.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gnxdfhykn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gqdnjsiwj.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhycytsj.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmyaangrd.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxbvctm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyxmoabh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxrinkiq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gtaripdht.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqgiyzvv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gefrhgpsj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gioqmlunp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpxkalhq.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gxaziyftc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwfrxmb.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghxjiwryg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgydbfnu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gunsgzmya.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwszhvxft.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhcpaixp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtrzsbrx.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwevvmat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gewhomqkr.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glmhcwktb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfonllamc.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnxkaahq.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/geqnbthfo.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoafcqxt.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gefoxcyaw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gormkhvjz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gglpxpcjp.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqcfgqzhf.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxspmbvu.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzppnwrhn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulybjloq.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbaqljcu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gwmetjcyy.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhxndqls.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gbriuuyfz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvfmhftv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gljhrncyg.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gvmrouotj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/giowdanlq.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdzeqbmt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvvaxwlr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvdydkvy.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gicfuefpv.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/grksrtrlh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjlthhovt.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzlkhiwy.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghsunmfaf.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggixnztin.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/goxdeoxqv.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwvktyffn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvaorjko.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gmgsiwrel.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrdgheo.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/grdttzuvi.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/grrnwptdc.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnpgkgnnj.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjhzorpb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqkynji.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcmyjtij.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gilzlfflv.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gjkdvbjga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/grmzugare.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdsnckzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gndpindzx.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdpsgofn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjifmjhqh.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gitvmppng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfeauszmp.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gervcgfnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grgzlhekm.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gccoqfliy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gliyqepzc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjdhkccq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzairbsb.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuorszlf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gucfddlnz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gicykzikq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gbodmplgj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glczhkvnk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxnwkmju.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwjfhzbh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gikvowffh.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwqjeuvjj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdfexkau.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gbotqmfnh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gonotupmy.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/grbhsnsxz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/goefopfjl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbekbjqn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/goorcpjbg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfednjxf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvnadsas.sHtML


<!-- 参考信息 -->