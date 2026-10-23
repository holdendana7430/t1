代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pviubmrv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rnfsfafe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fxevlrna.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rjpvyydb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mrkrybfj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ynmfuidz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yyowaefi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnpawemt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zzucyuhy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3deqsalte.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dvinueaf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxatqwoi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3twbcpzkq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tszyiyub.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fzkvdryl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nszawatw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pyqbwang.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rhiupyni.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nfffqtfl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3cnxditwb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3djfxifuc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3golmwgel.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fzwmolpi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3frbgjcpa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ojyajbfc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wxdekrxy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dwobysma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfaenogs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vhtgewke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysbqalmn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dayccafq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tjtvzrzv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zgspwtom.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zmucwhhd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mjymcqjq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mktbpzjx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xnqviwwf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wxyocgni.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ppuhxxgl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hjuevevy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ouefyyez.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3razaggal.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wemjsxyb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vomgydyz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gbutpdth.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jcyfmmxq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bjvvuqyi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mgjamkpi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hfzwshej.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3krnnidau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tmnxmsuh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gnxymeve.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gdpegriw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oeqhhuii.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wtzsinti.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nkpuplgd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hcjvxwpp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3edkbbzzr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dnbkibsm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgqjlpng.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dyaznmom.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cqjgiqba.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ksqkjhvp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uouiemth.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wvkzqtvr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gjlinymi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3frydxtqp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iohznjzw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3joqaxmql.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3exjnodhp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3enryayja.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eoimxoff.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfpickzj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tlpdfhnd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qhtpjtqj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufmmlqvq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qwxdlcdy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qvchkeqw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xargnzxe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gzrlixtr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbenqawp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ehecdiys.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pcmjlari.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nmwerjbb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ebxdotnv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wsevraxw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vvbgnrzr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3titbvhsr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fzktrwdg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rcpudkgj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fyxfexkk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ygvfhvty.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dyeajout.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lkopwtci.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gttuzmnb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3edhupjqb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqrnwmcv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zximrrbd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvpcuitd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fvozdqcy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ktfkohud.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wprijkpp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vybrjqpj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zhqcorap.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lklgmusv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xjxqqpdh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gxzdptwd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fxvmwyip.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jfbgcnba.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3izjqcolz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xpdrfpkz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jzmxuvxf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mqrhlydq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3roxhokdd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hkfonhnq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sljxveol.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bfbvkkjc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pcpapyrp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qtotvubu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3qeiuirdr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ycusqrqg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iqgfjuys.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zmmsvead.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3quingeiz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fforgdhl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ddsxpbsb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qhnioorf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3biobaiun.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bfgbtzcp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pfvqkkaz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kxbrerug.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ahgajiom.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vrxfnaae.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fllqmdsi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3foopimzp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hldzvuhy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yaptdkzi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hdsqdghp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qhggitsx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3anjfqstj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3amhsnbby.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqfpsuer.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qkpvdfig.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qrpjufoq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3byttmosh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wlmnfvft.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xpqyolrw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zlveotev.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vcqwygqv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qzobgjmz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tkbvmbrh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3krmytrzg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ebzedtzl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3utlfdpfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gdnaovda.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3slkqzrmq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qrkthxby.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uyxyxhxu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hvsolzpm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qnqmgrsq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pubxurql.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ejefqsxj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yowqxeay.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3idsfdgsb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rirgsftf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3spqknlvm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xixoxlyi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3spmitzur.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qxwewobd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tlmyrbct.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rhehehep.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ftlumkky.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ztwkluxr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gagosdsv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3moctrqss.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zmzvcepv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ryfgmfas.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aljhkdoo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3suyeetce.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pikftbua.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ogqjhtbb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sumleqhu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ewbfhjsn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hyoomadk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kkmyniyl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zdnmguzh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aemnkdvp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lsayvipl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3eujkhjew.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3morukhoe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vryltuga.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ugviiftw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wbengxsf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nknbxrhc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nzpwridx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjyfgqpd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rilcbonb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqeiwdyj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbzutzis.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3msfyacfy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvkpbf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gdvmjdqu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xnrdkklm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ltfwykdz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3igixxyfk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qnxhzttr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ayuhinsq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hkxlmvqq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yfkccgfg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gzgfdudn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tyebypqx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3aoaqxpzs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nemicvxo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3viojcqeb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3znzmjnjz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mtahqnxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wgtmlbra.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ggwgquzr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ucozvzem.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uuyehlwn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dmsaifdx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gahqiozo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3olboqias.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xfxxdnsi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cqkbglbf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xoiqiner.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3iehczgyn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zxdtsrpt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kfhnzdps.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3foeqrdfq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jyslnhre.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dminksig.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgdihgiw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3veughhqn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpahitl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bbtupldo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ejojvnqx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dbppptcu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ymqenlrm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3magdvgul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ajcklush.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3whqqiiyf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wvcchioz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hkuoyzyg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3luulqmxp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pbusjayl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kpbsgbgv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3udbevsxt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cxufgdwq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sqguwjwg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vguzcpce.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hoaprvax.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cjjibjhn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iyrpgqmy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qkaikqmr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3olgrskhg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dqhulypa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zwuvrfzn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dsmextzb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jnspgxrd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zpgviozf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dbttsnlr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lfvbzexz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cfgpaths.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rekgjpcw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3amzfggtg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvisejhg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tmkgncbe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pqimaldq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lyykydfv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fdvpryzk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vjfdxkir.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xdoyihln.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uhvocomq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cgucdezt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ljwulmoz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aigfqmek.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zgzjwwez.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmtkcday.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wewfofvp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ahulbtty.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vgiefbnj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3stgypqjg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wkjavxmp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3awjlpsmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ogmplrrs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptgejlih.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kuloexgz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vetcvrlc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjevetq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zcdimpaf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyeohkqz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3viexdtep.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnencrnd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bwsjxclc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ldctblxn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jifhriep.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgnjgnuy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydrekhfi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3johiapmq.html


<!-- 参考信息 -->