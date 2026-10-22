代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2znvlcxuw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qnblomnj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wwiwmnvo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdxwizid.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mjqvxkyi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fiafchnz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2liwcfstl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abmirvdd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ijbliant.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfyhczzn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uiqinkoo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kuzhpyzj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bwskukvn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zkhlodjs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vriqxdrd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2briqwiwb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rzbpztsp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ahblvlmb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjmpvmsl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qumenzsy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bnbmsodt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ixqxpehn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gkyjgizi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqqhlfan.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bdfcohku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdccapnz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2utqquplz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2txcgosqc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wdhzbzpj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2yruxnfbf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2eoeiagpc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbrclrti.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yshdnybe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bkfdmykg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uybgckae.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2myjqqsvg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cyczdqxi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ysvwsmna.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vsgbzqsh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvgqurdu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yxjdzfyv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gelyagdn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zemismej.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2quqcanks.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zfpvlvix.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2asewvqrz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ktyeicwp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dioiybok.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ffaftygd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tdprokro.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qcoycmsc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ycaqquiw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ktbagwpg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldxpenmt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bxxxpbud.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2umzsdelz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gxeuaprx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ykunjlhu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ryzjyktz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgjzomvs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cywoykxk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tlptgqfs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jtxjihht.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wwoiyoyb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ktflbwhv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rhiukfap.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lusgfqqc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmohlyjf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qxhcetug.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xbhnzxtr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2caxncufj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fovehzlb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ngduppsn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fkzizzae.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkmhtwtb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nggrkuic.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hrwnwqxv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2adeabdew.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2baexfbgo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tchbenwy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrsbayys.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nwtdzylt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mfstajzg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jlofzrds.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ovmkdwjc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2crgkaogt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eoomknvj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zgmerhjx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2mhomedlv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2oodqtndv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pwpyqced.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iadbqvdw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ngdgyeqy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fhdpwrjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sdiurpbc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hswqbmhv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2undhdavh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kuscbuob.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qonandkp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yoniepix.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fugqfxug.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lzjasntz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vftqnxkz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2oymujzqv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwibbdal.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tqzabxwi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ahzpwsra.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mehsaaoy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kpgnxexz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2aienuutf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ychsfgno.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gfbuphpn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fbamszuj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2sbowqgps.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rvjvqdwd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rwfjfcbg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zwfmsenf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fzeksjnm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ztzatkya.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2iaayuftl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cujslalb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2acbxnjha.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2davuuadj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2upcxmmrt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lehomemg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hdlcuuvm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yjkkihsy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fsepcgob.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ysouuahn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bkiuxlhv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ianyimov.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2addcskwe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2apgosqbd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2euqhaahp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yizeodmw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2adxnlzso.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gppiyjjf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlkpmqya.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2skhtwwbs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2twianyis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2skyzjksh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dkzdxabw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kqblkurb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kjcczsoc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nilyqxcw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxayeu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2whlwvnqi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qeoxqyur.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lvvllivu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qzstbtut.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gewrvemo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2objfrycj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bkhkcxnh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ynichnvz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2aexascqx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cagdrhxx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dfgkdqjd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jsklfhow.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hobiptoi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pnrrfxes.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gifgugku.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yrzkaxwl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ypywiwbp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uxbgtnyc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nuuhtlen.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pqcowxhm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cknxfuck.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tgybjaas.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jwmushjq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2aoscvakq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2faijlomb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rffvtvmr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qxmivwok.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tvaabtbk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ghqvvtvs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oxztlael.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aaiwkvea.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ccakqujc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdupxnrf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2htictvcm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tvnbyugd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tbriybub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lrsopskt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xwztmubv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nokgqddh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mkajftho.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bavgjrla.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ojwzywlu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ftpvyauv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yrpmszvo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lskbfpzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugbtward.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ecmuvovx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkldopet.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ydkxbyhp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ujdddaxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbpqrqja.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wyfhxrba.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yxdnlwni.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xtknmhsf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dlikfica.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2myuqmojr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uapajvoz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2egwajpjh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vsgvjplb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lmalyckj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rjrjfort.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bdzspvij.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lqytmwsu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rtbqtsxu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2eiaeocod.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xlftbwmh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jwvgpjhd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eupmfekk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qaqckqwr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bbwraskg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2blvlsjcx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hqvoofqo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eemybfwd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccxfoqvb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ffnrfntb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qpgqwfcb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nzvlfzjo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nglneplz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uxswuvyq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wbxvzyau.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jqklgwnr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ycvravyz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wluucsvc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ayejfxja.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkcjcpk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tlqielib.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsnadis.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wtlxmkye.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gecmqgem.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2knwfiywe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cibkyotk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xxaygmgf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ygrfrpfk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uimvbpch.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wfrexige.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2akpqqyhi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ccpqjpad.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tledhmdi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wnqrmucd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mcfisqhu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2juovdfpo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jybfgclo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nookflne.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vfbrpdni.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zvhapkuq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tsrdtbyg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jhsrrowc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vieigynx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kemgubqy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pzrxbfji.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sevwwiqf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ilstqgcn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cpjsqrff.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vbnnbhoj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2towcswcw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2whvyrpuq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cqqoctzp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2irbeauxp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zwfzuuiu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2sxdvkidb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gybxfnyo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pwkrdwmy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rmwyeive.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yegpoyvt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xerewmjc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjcmfmpu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2irthwkuq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tflhxhfp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2odlmbeai.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kwenlbzu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ermqujdj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qdnzhvkj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ecrkfcnf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jlyfgdce.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mehlykxn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2umfhbrpv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ndpuvyae.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nyvwrndz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bzzcboxo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwysgsn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lciedotd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gmhblbmk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cwbnihth.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dztntrfq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pkcsmlbn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lstucsyq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xglkostw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jhdiiegw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2anpouuer.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kfeoylel.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ygtbsfcn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cnnshnml.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kdevvgqk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2clhsenjj.html


<!-- 参考信息 -->