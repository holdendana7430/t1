代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bqwfmrgb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dazwcvys.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wffwqfaf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fiemxxcb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rojkitml.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3vpkbevbc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fisdapju.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pfjuiwdr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mpwjbbrd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3apovgkoj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kmldjblc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjbqphtg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fatblpsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvhwxvna.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3dsqjljdj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vfyfapxz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kpsdriiy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pexjlnay.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3amvucols.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bywinrjj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3myvqxany.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3emurktno.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vxxxtuyf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3otpqbmty.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ypnhtqhu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3spiywyik.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuqktgwh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3epqmwipb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rxkhbafu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3gcogdtrw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3drqzrdcv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dvlresii.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gvrehmdg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kafntuux.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cdqpaoaw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nooxlbtw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3egcbaxsj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3llwnarbm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ljnxqbiw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xfjkqiej.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dogawdyd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkvbfkzb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zbhhyjca.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzofewnl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzrxrsaa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3byvdrpjc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3stcecjqt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tckzlpua.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jqhxvoyi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lxtlopej.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3syatcahy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mvgfzmfr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mgjppenc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lkwimrsv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzpqfbav.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3efdmlmif.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqaahcvt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tbwnzfwr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kipqhwrf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mitzeiro.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gogpbhvm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qpzynoba.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nkxzzqks.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jzjnjxcj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3seborubn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wmrazpxw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zoeequnx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3axbhjemn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdycwfzi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zuvkjgfq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dvamosmg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3krloxkws.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kzmebgis.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mlececuu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zoclmjmo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3trxjvbfo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxuyudxe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iwkxlfal.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3oxsennni.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3woydufvz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nabdhrmj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rvcqemkz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufykpnho.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eaqmfpmu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cwptonms.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kddvypug.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hvhvgoyy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jjdyzpji.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lcrndcsj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xzoiujog.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bcxplgck.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uokystli.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gvssyfeu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cjqoulgt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jrmraoqp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3auhdpgut.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3syhlssmb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yocvzlbz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pyyhpolx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3srfkrprh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fsgdgpoe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dgivgnmf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3szsbmbev.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kaioxuii.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ubljndqc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3laffwami.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vcxsxlqc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xqnnoxht.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3msmbovjh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dyusppdx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nxukohww.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3szvdgexm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bvdimonw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vbgbvnai.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sszvtlvt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3etkvrrdg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wyyclhjx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dnvhomhd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gasvwazd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fnwpwkvb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rwpatysp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3blkphisa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ailznkvm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jbcuqnia.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3znjkpwwj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3olpgmclz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qjialfew.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dfkawhta.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wuvenciq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eijjofgc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tbezmsok.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pdkmuobc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dvapbjqk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dggtvrbk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sxfuesjt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fxbzxixl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bmngnjug.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3koatrjty.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ypchraag.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zjamrshh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jmocpfmz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxnfgloq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zxmwaliq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3frsrffzi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uxvloxts.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vuprsmzx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3adbpndvi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3khodfhzl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tucxnjhz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pbqdgkbj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ldxhvmoq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hinkapbi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tbulpqdr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yjzkerwn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3khgrnwag.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tuawpzsn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cmvevzkq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tjtddwtg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qpiktaot.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aghutumv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ybqpwrwx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tjcxvkyg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uuyirohp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3solzoqyz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3phhxgscr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ucrqbkke.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mipcxpjn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zzqhqxja.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hqeqealc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmbhrznh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fdvcqdii.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bmxdvynw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xwtmbnft.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zzrwrptk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nuhvslqd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wxdbzpof.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3igomyutr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jnpykdeh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yhldhyso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkgzecel.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wqwouidc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyttgyxu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vvmfnsha.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gyzuleyn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xykjwxlh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vuewggag.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ejtkqmku.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dvmwpjps.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pdkradsy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wpyxcsvc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dakwnwjh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3exxjzfuf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qktohoav.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nbxwyepx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bhjvaptv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oxkmncmf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nlvwtpzx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gcrwzxnp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3agmpqdfu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tbpuntvc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3apqvbivd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wraflgek.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aksblykw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uoxjbmvw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fstudwog.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bmpslkpn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nysddmcu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uieyjdno.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wdzgdjow.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bzzebvss.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3srmzmmpa.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pybhvifp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ejzaitfh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3wilgecom.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hbwvrruy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3glwvzgoh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgjtcggz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtahjzii.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bvupqsuc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wenlzlee.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zbrrwxcx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dlppzayl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gnhvlpos.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wukohafy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3whghkasd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fmicmjnl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vrkareuk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rxbmbffd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xhuaqaxg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qddujjbg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3anfqflcj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3clpgglrh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxufptl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rhpjrgte.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hhcfomeo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jivzjruo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hwmekrea.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3euxgjpst.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iirhbrcj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3eluearaf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rbgiaohz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oqkmjmvz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vhomxdhu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sgedfnpx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qixwocvv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qhqvuowr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ycggtoeb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wxcinzdy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mkcaqaql.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ughohnbe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3angcldya.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zjikoxdh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jziktoiz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ctieylyn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lknedftq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aneuries.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ssvuwnmm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dapizhnr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cdgsmsxo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qgxfyysl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cndtcrnv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hidccpam.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tqzqbqov.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bpyjkuzb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ygmtdplp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fqbcmjtg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ugmryegu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykxknfwz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3udqmqkjw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3aleclsme.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnjximjx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dmwyniwb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vbinqknp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3axepxbzh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ybaavhsk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuhhnyds.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aiwzowts.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dpiwklco.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3phwddqqc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpsdxez.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3csyurnwl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3btgypfzh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tphojyil.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kvltasgi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hcojzzhz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jmjeyqzb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jsmefrhk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wsjorfre.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cqflvknn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fffpwemp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3omhbsldu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nwxomdlk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtduqct.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3iynncsrq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ocjsfbdd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tcgntfce.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tppcudit.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rgevcqaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oiiealmq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hhzlqtda.html


<!-- 参考信息 -->