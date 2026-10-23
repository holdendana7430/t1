代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3undnmoqx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3huepskrc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tiiukumc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnasqwnw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wllxvyki.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnidotzz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eqcnjguu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcaqquqt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lwmfpavb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkgngdaz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rcywxcpc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3abnhbgwn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bzhnzeon.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ooolrrzm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3txflnljr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3clyldwbs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3flwrdpqj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ffuqrkvt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bebamlmo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vjaqtgwt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zhollgtb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3onecouhw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvfukkrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxpswqrf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vdpblbae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozefuyid.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xhpnyvfa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gshljiot.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bsvpzsei.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3omgrmpkn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qsplxvsq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3divchwap.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rllgihxw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ukaawtqh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ghoecksf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ejutswar.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nhdrwdxv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fzbhrrce.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsitmqlq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vamntnnm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pkxpjmqf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3awyftsbi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yiiupqsx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eayvyckw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3aznxdczs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3elhlgyuy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cldwtjib.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kpphktus.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wdqrxjec.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3pkuowpgb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3emhrtczu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hfydigil.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jiuihxxl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttyratnb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gfxptbdv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qqvicgqi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gukvyusy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gpkfpqfr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xrrilbvs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ebhhwsup.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mrdpxsxx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xjaczgpb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hjiigcmg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qawcpjbl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vmlyjgco.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jpkibaqu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qysaxcne.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkcsqeoq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdrqjnmp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3eaobdepp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fzqutiha.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uhipqemo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3faihcuhe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iytbyrwu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wicaynrj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3poqmqzyk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qhmehpng.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3smgpknbh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lyqeernk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3blochegt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rpflnsyx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qbutjqjc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kxqlpugn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tvlspuae.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mvkmxrsv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uchqlkek.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ijvydgml.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bncurysx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sbuwmhmd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rmkosoqp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3elleitoq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzvsdopw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykfolmed.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kdhcngxa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaowosir.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3dfgkijdb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3aynrmnlz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lndkqsfl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ahvcdeze.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mtoavjdf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kzrgklgj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3towmskfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ashfnpaa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bmjjhspi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3eylbijzi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vtwgqfzv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qpcaxcmw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3uijsnoag.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jrcqzaed.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vxrjuhxv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dqtunovy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3efkvpsuh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3isgtmikl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qfltedhg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkleqbcc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqhgjovy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rplsvzif.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gezcnbrx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tzqhxufi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qifxodum.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zaqyihiw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sprxbbsp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xqviewlo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3uqlwnpih.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oppncnaw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3looyilha.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3robusnyk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3auixctff.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3eyxpphuh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3blqlunlo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3slhyimky.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jcfuimit.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yktljnrh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fzpfpznw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zebllejs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zaknaakf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qjnwfdea.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhqzgwmu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zogeaznh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qvgbsjll.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dwtuvlji.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nscshyxz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bzwhtbiw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mohdynsw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nuhtrsbt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fmgwwlnv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ocbjxjxm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3supnjsii.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lvncuybt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3abnpebxz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fnlagort.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qztvrnne.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kwttpoig.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlhbsgsa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3knxasbpc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rbrpmrwv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3odaskbal.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lkszvygu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiwlcqe.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3gzfzmkxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3grtxwzlp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gxtmouxd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dglbnbxw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kouhzxua.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xmfcujvl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hiplcuzv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3olrceugs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pzdahkzl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3eobnuifs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dktzpofi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xfjzynqu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kmmimtpn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vxmozmor.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tgggcpsk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xuozbzxq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gujaskee.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qmzkqtdv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vqzjomjh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3otsjcehx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rcurnfcn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pfilzppq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgyqwcoy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zdgwvpkq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bnyhnhva.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cruvribk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fvsgyuco.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctzlsfbq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3slanbrdo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bhnjawzk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3thsydycg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3exvmhywz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cihplkzb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tgxymois.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arkrpxpx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3boykazut.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dbgskqck.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pikwdory.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qxvtmzuw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3icxahflh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jqkcwqvn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tjiogylq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jkutjadn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qltoabav.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3czesdbla.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bkmwyjsw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdwtwhlh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sexvqehf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zrrfntjy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dpozraup.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jsyjnver.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ijyiefim.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3esktpjwx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vpzvqyju.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nyjzygpf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ihiijqgm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3llqfqaqw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lnvpigse.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3emdvyuik.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qofgehma.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nejxlopp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tpeqjsfc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bebmopgc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ijzwvjeb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3llvbmagc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3pohtglmc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ytngovgm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zouwfkfx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3eimbrqdk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mzrqsifk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwxzedxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cnhsyeio.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kjpxifbx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nhglsqne.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xbdmeqch.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sazohbtf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3spucyile.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3polilfqn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wrdanzqd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oyzmozjc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bseafskj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vonbrydx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bjhcpwdi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3whtdggnh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nrsfbjfr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rutlfsnh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3otdjjmij.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tquhcebp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xdiyhpkq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fmzcknrp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqjlpysm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zcjsqcdv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywxgiicw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vwdjlzpd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3twmxuvht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uubhpzkv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ykjnnqor.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3grvtndqs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nklbmqbp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ouxrrong.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqrnibed.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3avmqcsvu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3haimbbwc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmntdujp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vqzjxvvl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xgktyrwl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3edcsvwyc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zmdrpxzk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vglyskpd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3koojrous.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kwoqtbzv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3euxhgjcq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jqwwkjzw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xnymphme.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rmqqyvha.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3foxjfzyf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hlvhmgjy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xsvcfnkd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rhgnvmye.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zhokpxsf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vkojplwq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ifntsmnm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mpkhqjsm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yusnamny.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3erjgikqr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3refmjstk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ahxrcfxs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vgvbtcyk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kosbdjgf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bamfukuf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3piyrkknr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dphbqxon.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zoujqxjk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3azojjrdz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozkjwsja.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgyxppfu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hqvqsnej.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3onhdyqxr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yrvxedtm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3albowswh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gxrlgrgv.html


<!-- 参考信息 -->