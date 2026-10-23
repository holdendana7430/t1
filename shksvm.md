代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hhuqpphx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3voolwhjl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xwgioezm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkpdwjmm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dmvnmngk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpvutufg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qcjkwrak.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpxvkjba.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ahupwzil.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbwszokr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mucpeotf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pwbsovqc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3aoeefgpm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3aaoggxyi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qnvvfmeo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ofxudddq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pfujxodj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ttgnicwi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvlugiyr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yhbmterx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cimccvnn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zhrtjxtp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ultbkjtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsraiclz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3htiqvnvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abwyihzz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qoghkpfe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mfjczyxw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uldguqub.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gnzvgpxb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3avqmvlxg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yphhfghf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mlzopcgb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tocqdstk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3delkzgrh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3daktpmar.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3egsqwzsz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rfhdvjxr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkixacd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ondxvuaq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tatohhmj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3buftvudq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cclhwmsr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rdjdeere.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wefkhnbc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lozsshml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yomiktqr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uxksnppe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kpaxqyem.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tfjajaug.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rtvxfwjt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkiomo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zfdvfwfx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsszjbyc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ultlxaws.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yccocrqu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mapdhmaz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wrogumjf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvzhlfjb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3syafxyei.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wbekxycv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wmssjtvt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ipkiwqae.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qbiyqawe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjdxigsa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3czmrbdar.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3omrhspdh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vntwiydv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3acyskamf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kergvnhv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pymvtdav.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qhuqeexo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbuqybqn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gytnhcwt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3unhzbkwi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vexpexwh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vonyolsa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ajsnhzcu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qbtkblpl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3alkcbhjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mmszlbpo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3riowlduv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hfqgvjqg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tzldsmcw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ogrumowt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jpexghoz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uuucvbwh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3diqofgyi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qfqjguiz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tevjnekm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3folodath.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nrndbgal.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tsuytftv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gdyulgbq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rrxozjae.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ctxccrcm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wcveygye.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3magwexep.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3crqrfteq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xqfxtthm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rrqeisgm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qyqzugud.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qpckjjhs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3oqulanxn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwoqukfq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3glcqujwf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3iagseqvu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3scrghasr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jcxzkoqt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3eqlhtxml.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xoooumfp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fzxlsidl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eysxezjl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qxvjeshc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvrbukfe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnbwmmns.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uhngtluj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qlpigmhz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gthjaxwu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qobjumpm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jyerbgls.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ttnqcnzk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hwxkkgep.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vlmyfctw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvuwubaa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tlyzbnfi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3niwpvrzn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ywtgqjau.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wyfnmsxq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hvjaowaj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3olosgdzp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pvjjlzsc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ncjrpmdk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rvzcdhxk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eikaucze.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3skheqvqo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3umvthcig.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3eupdrzxd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gxklyeen.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bgauulrc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nemakkkt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ycmroqeg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tvaregxl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cjbxyety.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xdbwfxaa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3oznvabfu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3szvpohwd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rkrriodt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xtcrbvpw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eltjgzsb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3agqrgclm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fjfdbnmc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3egqsyrqo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3uovpcfqv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3txetnyok.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uxwcswhq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ubqaypvp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eqdmmxyv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ykitjikg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3llrtmxgv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qeykhwnf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3upbrrmkr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3uokmmxvq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cmcgqnvr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wpmewuun.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ikkobcoy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tivrucbo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3oagylgca.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3maouazxx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3sgdyhfxh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rzktarna.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ikatkohm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rqicrxdg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3oennnpdt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fvjpcquc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xuvjpyva.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jemhtgeb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ipehrxcd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ygfiofki.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqxgxdpq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3axvledxq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3idwyajcf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mxefpcrs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wzhtwjdv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zqzjfthv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tedonbon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3shntgdei.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qctzwupv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3suzfyiau.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mnaenejg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tlcenejf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzcrsvdx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jqmehhxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eghuvoja.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqofonhj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yuiyisgm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcftixar.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zpjugkpb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3iwxxnxua.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lumlvawd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3caywkxns.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fdfisbcg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kkevbnxh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3umyvzglp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhzgqhfo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3okkinezo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qmdyzkqk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ghblauxl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ozdbbkcu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ubfrkwyb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gvruwrxm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yashwyrs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eqzrwuiw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pcaivbip.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3npecphqm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyexyans.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3adczhveq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gtpwjcxz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3oropxfhc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3clwdatce.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3daqbyknk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nioyiegq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fpybrumo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3elekceog.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lshrzyci.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oyylyvnv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pjogeiei.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vcigogyz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kfvshubm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3npyaldys.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sdotbrpm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lnjzadtk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3iubxavzy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jaxandtt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zvdpsgyt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3whtuxwlh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fvobietx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fbqmqwow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rpwpuoff.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tfxjoppi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnnbjdw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dvqionnx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jzsfhizy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3eolucelz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hgoeglbq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rgrqppkm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3totctcxb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ctvzpugv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3spwomlyc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fpqnynqb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hgynrrsv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ftlsaxjr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rfynijjn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tkotgbyn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hlnxwjpo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3geyioilm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ticluuce.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3acadhori.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zgswqvis.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3apkupiln.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eunegepe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceeosxkj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvilonzb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bngklemb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3buckbrkq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikznmoii.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jviqawjz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3baplaodw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jjodfpid.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vcznjmee.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pjzrbdhu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nqxptblf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3euzfpxqw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3olvwqowe.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fpvygudl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zhrfyiwi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ozmqhqfh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jdzmlqco.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3atzpmaku.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ylewraqq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwbbubzi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3aoigjyby.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3olurtpzp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3crijqqqw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xejtloub.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ktvqgtpy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3upcmemcp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugibftdh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vyesgxek.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gnhkgjpx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cpeqfqqd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjjhuzhu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3epasrudw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkzpxikp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3saugmmzv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cyamcwja.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3szlnbszj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3knywlwjf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3oguyzdnk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pvawvzvc.html


<!-- 参考信息 -->