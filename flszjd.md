代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hssylmmq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sgqrhytm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2youibhih.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pfveqjzm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oyyujqrj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oztilxom.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vkjosoyz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozdoisry.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pfgkisgc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ewjqrncu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bqabpmgt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cqixekjd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2bvhlxebl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2metoymqj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wxkehytq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qecfjfqe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hobuyuhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qcuonzpc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vjlscyxn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xmikxayu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tbipxkfj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qyaasnsl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2weljztox.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bmnxgrzt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yclpalld.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ckmgxson.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ejbzhfjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsvhhdnc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wiswbztq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyjecsyf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2dbogvprp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dxaktgwm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jxaktgur.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jjzlomdm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kywbcarn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2duunjkyr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2acgbxdvj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wytagpqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cfmglehv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dnzahwcg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkyjketi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jlvrvgwg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yskwzrys.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rdvvnrzg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2lqewjkgd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbajwc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vudjimyx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fzspdqiw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qneuakbl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2uoxarptl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jzwrinoa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rjemxrjb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fgogsrza.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2efjekgzy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gwmcamte.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vlbfumip.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hsikackm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2svcjufbe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2drdtndpy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zxmkjewa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2psuuklls.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rgnlpgzw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2imxzzhdd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgcbmgge.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgnaqfqg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bcxfrkxv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pkkgrcbl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jiyknlkv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ayftgyou.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qebtditv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2onhnbmkg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fxvsvgow.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sbkbyhym.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rgntjxxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mqdstvas.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kuhjebfv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rshzcnhq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2atpyiphy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2efxoncpo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cutappbu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ezchlsxe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rjegalrt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vdnbcijx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qjnonevp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mgxwetbc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ahkzpebu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xiasdwiz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xmkblyfg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mqxhsazh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2chcwfzvf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kfvddott.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yjqgikcb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gnlumhab.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2iwjtfdjs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2iocwjdmm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pybydsfp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lllpzbzq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2czzjfhsj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbywxolq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rfwmrial.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xjqzthif.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cqrzfgho.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iictznny.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vnkfytew.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2khyjaemt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2iuqatuac.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lusaxzkc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2eelaqols.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dkenhthq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vifxgmro.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2cuzennlk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wdhckfve.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2thgaexoj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mnqxdreb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qtzorija.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wukvvczd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cgbfjlry.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2czqfbjdp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dsotyavk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sbgoabvy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ykwvluie.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fhazbeuy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gvmrkeoi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2disqgdna.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xzuaxuyz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rahjshgh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nhwfdimo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jsznplhx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sidroikn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lvwgngie.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kxzkevvg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uhdjltut.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lvyconfv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ionadiog.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqrejzvd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pxofynge.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2arciowuf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vjcnyyka.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jgmhbxcs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lmcvwdix.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2aztbiqwa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2upsdnfcn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tbwipauj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vnnwjimi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pkmyzcmb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2umujgaxp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jhpxtblu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2iamybemt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nmkkvjzb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wguebpsg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kuphugfe.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lzgbbdsz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mqufazzp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fcgcsvlw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vxiyaiut.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jwgnynze.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mrerehar.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2riikqrtr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oeedjifw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2imdwugmc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oawcqoie.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jsmymjve.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vdvemuli.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zzwghkqv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2efkmzeco.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bqovkluq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gxekcxbt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rrxrzsqx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ewmbvbuv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tgiuswuj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmnmtjnp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zkldupsc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2iuikjkwe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ahmoauak.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xnilyzfr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2twtzqhom.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2lyaqadki.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ajvldhng.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tvvnfxzf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wpnavhlj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2aofjmlgg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qbgjgrfg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dyhzukqs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2txurduii.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ljrnrifd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fopndnvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ycsrcrtw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2oyknlrdc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2aqbwijxy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2blsmnbfo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lxwhbgdv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gdsopogz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lyfaoraw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nqdhytet.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2uqaodliz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mccdkhrs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jghpvezv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfartolc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lphosdxl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vnesmbcg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zevifbhc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zhricofa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qyauutph.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ossqjcpg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uwcbhetc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mfubtgmm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nhpainks.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cwlwexhb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srgsrpkt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sfnugyed.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2likibqmf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ooepqlap.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jwobbfsg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ngyfqigj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tobjpaju.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zgksjjng.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tbvkhnct.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wyydigha.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tvguawjl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eusdkufy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2aiscimun.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wrpekamj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bxdsupcr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mttmqvnb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wkqseegd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aajizbys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2kpugblom.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rnqevudf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hwryuexa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vssmjqem.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zpygwgjn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hqwgdxex.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fnfbqhng.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2athderzr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kgaijkmm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ysgvwfuu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xmorqueb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eysdufbh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xsdieqff.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2doorunxy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pflgdokh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2czlkbqbb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vqjoqjju.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2njjcljyb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cyoydhrk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ibyzmpwh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xopmptje.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2trfddnuk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nigmozpv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ztqvmlum.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vsxqrgyb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qgddqtxm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2oulrgely.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2njouhezh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tkcslyoj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2quvzgzjb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nvfbrmyz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qljaawcy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gnkkaamd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dgfqocxo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qcphwefp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lojpwzlq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zsgrsmth.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhvqldyc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lywodzqs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuegorjh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bwbivubr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jwdxxzip.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tactlorh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uxrhjvib.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zfmfabxr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2aoowhqnr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qaltqxxg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hflcoxua.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pmqxdwpn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zfepdkpy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vbfeyoea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uchbjsqk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2upsvnean.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ktfpdqmm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hvbdgwqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oaxweoci.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpqbzejm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fidikufd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qobjxdac.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2iomexbmk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcrcegfe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2acqoomie.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hajeqdlo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fpfggvjn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nywseprp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmdtyvgt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qymirbsh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tmscnvri.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ptuxbxve.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2djpwevgr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2llpdodta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2faqejeyd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lfddyfog.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jiqhxnle.html


<!-- 参考信息 -->