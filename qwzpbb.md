代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hibwgcmv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vamvppkq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wbijmhvb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcldsbhu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3uezmyryq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbgzumxs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fmhdufvq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bavioeqs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xnqocqnd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scdnyvhj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ytzksxvy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uenqnjuy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kcolyuen.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3yhmoqkep.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3oaqwoyyu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3oryrvhmd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zqohzkjw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3skmtwczf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sdmiwoeo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qyhdjtsa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hqburjam.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oratenin.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3myfmknnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkdmbpqo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vvzulgic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3goolddlv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gkzhsorz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3sjwdbznc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nuguaqve.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wsligfar.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3idxpxiuy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wuprioqi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dhkcsqxo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3kiagejto.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yvhvtwhb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bntkwzbz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zncuqrta.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bgoefibs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3antldabw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gkkvnqux.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tllnxjwh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gdiwubob.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3apumiges.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3melzkotq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yvdkmoax.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3abpdaois.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vrjldwsi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fqahxnxk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pcmtqphq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wygubbgb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kaktpxiy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3pbtinpje.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ccoowwre.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cbqybqfd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3brxfeuux.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3huwpuflt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ftqwkihn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3juksfhah.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3douorgwd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hihlvtyn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fnxbzujx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3iursxngy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hfsvtqbq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tikzinjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wauomlnk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jqzhzfir.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yfdnubyy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrftztdd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ulvpyutz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fodxqsug.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrjrbrpy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rpzgzlsc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3modsayen.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3enwtpqhq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vhamumma.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bgevuqsb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zwjkzstp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3obzizlgs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzayvoep.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ewgqptqv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ityganes.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fvjgpout.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gmwfylli.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3idqfkmhg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xgpcqvof.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jvyvuumn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ttrxabzw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ounzhmhn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qhuaypyu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hmeascue.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zfcwckzg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhjdhjyh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fgehbfie.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zbpecuqy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmmxyhse.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pnlvnvkf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3csabzhhm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3njhlbwje.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bzcupjyj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fauqkabc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tlchkjrq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3akbdoufm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dttsvxgd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3aaoupslr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3blpjvqxn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dzhiqbbe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xxdcejot.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pookzmht.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ewdoouwq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mtypsclu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kwqogjkw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bwfzsifl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sxrzduln.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pyvnscxm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbrtcksw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3splwvyne.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cjsfuqgp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ffljvnvi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mdqkegkx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3iknezewk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3obathhcq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ofitjqxp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lsslvgig.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3namgggru.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3abytcbgd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qdtglyec.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vmtnetmr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fegbtxqo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3gxhwhehn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3homjtkni.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywckqpoy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ktcktdsz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wsprxmtw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tozsqrrd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cynmtfek.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gxuimqxm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hwlonnpd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mqnjrhvx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wevwtkam.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kfltchwi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3urxldewb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3iwmttsvx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jwhybqgz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bkasjvqu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ebvkpmji.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vxpvhyek.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cgvrawjc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ikgrzzdt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dnccseta.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rimcunps.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ecyltfnu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wttgtkcc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gaxwfsik.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiznisox.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nplddnbo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qxrccqlr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3teeomwhg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cpyscwil.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vbxklgjl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wllnthzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xsrttxsx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3odftsrrz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3uffabfjb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vtgdzumx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cwncsljk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mzwtabdb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gqaskzfo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nuxpwvmj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ycjaucrt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kbqtekgs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lqbalxvy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kqqgmkab.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xypucrwg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3cuqyhnnl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zgpoyiky.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ogsghapf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hvkzvdzr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kmytwldl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmgwgbzy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyktidcl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ecygpuxc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcsdvazt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jrychbba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ohzvxrer.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lmpiejky.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ahrsvwko.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fwjxbjvj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bscunqib.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jskgtjwj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jptfbbxe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qaqvaavt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrpnzqir.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3inrggsrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqmmmukp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qcrzkluj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rnolrspw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hwfvgsja.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mquqljmi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oxbupsqb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ihoqydsg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cienwoyc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hvqyisrw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yrkcmgdv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wjljhwux.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjepytb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pwopnwys.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ngioarzy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3scbotodw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3itswxwnv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vwymqrph.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hncoonoq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ruaibglf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ymxkgmep.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pfqukzvo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ynqpyxdx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mwirlqki.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zgyzgukq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tniyvfvy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ttidqevn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxyrzmrm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gfuofzrn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lpzwlsmj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vgbxddup.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3muaddfmt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3eymopmwd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vjitmjxj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oxltvjbd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eoatggjs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwauzgx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3phqlqeeo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yexcoxib.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xgprhznd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3herojpux.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rodjpszj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3oylnxyua.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mhflckiq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ssrgqdqf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3exkoutfx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jotqwhrl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ijxvgvim.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ruzchmda.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mdauzstn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cnzrwlld.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ldmbvhkw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qzrnkrxr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tvgcmhqk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3crdqjerm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3slydnvlq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3crtulkkx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rgchocna.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vftsvazi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3onejkxcg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jevvqrir.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdahqopr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3faoeywnb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3afrufmty.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qiwbvtft.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lgzueucj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3uqnixoni.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xffrgewa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3varoohjb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbwkwwle.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3tvlbouzl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mlhajwan.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pmrmveqc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3addxsnxk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3iwhlekrn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eectqwul.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kolulwwz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3obbcvxmg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3esdiubtt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfmqdems.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qmdqptyf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmmhvlod.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qbyhvcyb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jolygknu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xwcuvjon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cemjllry.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bkyahfko.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lhodwvio.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3afeukznx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ozmqnhlx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ialnelqb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pvbbyhas.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3azgwqmdd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ktlpncol.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3prjumqdm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxacdhf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nfdkepph.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nzwbihbe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3usowyqja.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrvnaydl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3glhcjjnu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbydzxgq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iuuxpqxh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qafyubwu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bwwwlmkf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pblkwcxj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3azmxlcui.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ubgslwbb.html


<!-- 参考信息 -->