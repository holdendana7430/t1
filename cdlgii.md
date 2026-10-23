代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jrwyuufr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bjdldpuo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3owfxqkoi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3teaezckn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uyiaioqu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvjpunjb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3skkuxtbl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sxbvrnge.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3skxnswfe.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vsjmkdch.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3iiekdwwz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fasgbswq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iivcxoaz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3iroumtcq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bfudqvbv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pcacksnx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jwgurhao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wpwwhkfb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfbejvgh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tefaivoe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bgrmblxe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3omrknatw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lmhigzvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfpktcrh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vdurjeqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqktvckd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3feowlwvp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tbbjzrxz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vpadkwwf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hsfwcpac.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jtbamuxh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3iazqqibs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3igysoqnh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sezokydo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rceuesyq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uygfqumz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3abujvkig.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cujkamfk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nokwlsri.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3elftqlnl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mvwenets.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ulkwdrww.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gsssxfhi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gzhcsasa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sitluqea.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ckrryjaw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tzvimwcj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lhpjjjjy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kakvhule.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3czwoucms.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bqbwubzp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ntlcmemi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pclspgda.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cezwcjlq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3uvdnbdvs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3shwfvojm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rvdswyxx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3sgxwvomh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3loazhomz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjlcexow.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3apsmyoil.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wpzyiatz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzxvoiwj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mnkvwamz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3akjkapic.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wuwoxnqu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mxwqcmkm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsnozzfn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3srrmnfog.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wkpxeafw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3oattrxxb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tigflpxq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3effcrtuv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gqohcxzv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hptlxgtc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tkhwzett.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vnthnzxb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fpfqtjqr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zpmgrdeq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jfdpkuoy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bpwvcqst.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zgldzdsc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wcvkzmca.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rnnxrlvl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mtbsjdyq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pehhjxyh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3earjrsei.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3irzzwbrb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3aljjigsn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vrnpygav.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ckjkxvjn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iyqlbzjg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dqgvcofe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mwekihvw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bhzfkslb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3agloltjq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mdfhsein.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sreriicg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mwgrezgb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3znasvaog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gnnnihdj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3txnrtbum.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3glpjunjq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kjmgxtld.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rvpmnhpr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lkgfwime.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3niwityek.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ncsctlzc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wjlgztbb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rgbzdggg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qivtkbjb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rkwokxly.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3faoqzlxh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gvtfszxz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cxuqpkxc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezcuzyae.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3etgsqqia.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gnnquafl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cpcwcnyw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lgldpyrc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xouqfvmu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hisjntou.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xbcqbnde.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3aqdnjkfc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3brktanue.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dehetywk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fgtinptq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dkvavfbo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ibpjpcis.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mkrjcltf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wyrdxsqk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vonjrdyy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tsqhycnd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wcojemrl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pwovwwww.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mvhqbcek.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kayasmvl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zgnriqfe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eqemzbnl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jfivfyka.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rjyajhwx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kagxnjer.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yoggledr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3plovbozt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ztpemqvq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vaqhzlha.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hktvpkbv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zcxdisfg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ikvohkfi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xlmeoekk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ivedmmro.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vknkwmnp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3equjoukh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqodnrjc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vxspoqhr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rmvvhaiq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3leopwcim.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gldabaym.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mzwxiphm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fjnbqekw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3whwuhxhh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ehfrxtkv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xcccjrwt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sajvrnuw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hclwmhdl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3sgdycyaw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kgguaurc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ifpmdvlv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nlcnwyno.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pkqldcox.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ifjwzsgz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ovqqoljh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xjwgwpbt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3shpysqce.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xsopcdxf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pbpiftfa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zriqyqjt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mprrxnox.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3iotilsns.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3guyyowte.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zybppybx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ibrmxwew.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pdlrvbir.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xclrbzpt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3chkdiirz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ytzskhch.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fyieimoc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mmwrdrwc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fpbjsehu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pcafnqki.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kcwliqzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqwvcmtf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mcuzpecn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amslpizt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eniuyiue.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ifyufwbk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojfdjupu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xthrodfx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lirinuyr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hnnguxtc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpzukd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iufzyjra.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cszxperv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ckhqxnpy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcorpvb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3oqgfhmta.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3brngxjge.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gomdaaag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dbyhgtvp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3okpotbxe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iqkvtkxn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yfdlkbvr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rgeubthg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ovlcjwtv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xeevyfmt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bmebapus.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3syyekjvm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qczaqsvu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tsrjpnjb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzepltvn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mcafoqpn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wadueeck.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kgroimcq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3sblgqtnj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lhapgpfm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cfvtjiua.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zcrpgzpr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3laiyykdc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3oirgvgag.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3csltsdth.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ojvxjowk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lmifrlpg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ycrafbqd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gwgjhaxb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vwiaoaem.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bpwcqqtc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3proslxgh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hncmicwu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zhyeksyk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nauniyga.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3frwlixqe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cbfatxry.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pyvpwbtz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yhynmthh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pvevdlnj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hqrrtikn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zfbpmweq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3eytqppih.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hmawoefu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jeypwrjx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jyotufzo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jgxsevja.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wbxhwnpi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gphgthkf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vhgelpad.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sfndmejb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3drjtopqr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zpwpgmmb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3atxkjxxk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jbfqjwtp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cwybuqkg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxmbazoa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jsvrxknd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wzksxxgt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bgjmoxdo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fodzyzxr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gzlluotq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nnvxbvsd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ofuetbin.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blabytql.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ceipppke.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xyoojiol.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kmqjwpji.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mwmizele.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lzjvbdcf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iuceunef.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bezaizly.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dwyekgrm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dcehbszi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gvhwblnw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkjlncao.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsnxotlx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjbpjtyp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3uwiwqoch.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zivqqvea.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3faeuqfgu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nlmmmefa.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kamrinhy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3crtpjjxt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mhqdfjej.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nqzaqetn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3efovpcid.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rirpewbx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kjcydzxi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trmwjmxg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3obixqphg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vviowrfm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgwkbipz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bfbcnxau.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mbayziuk.html


<!-- 参考信息 -->