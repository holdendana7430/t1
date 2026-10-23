代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qsxqevap.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tkpevumv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylnjzfjc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fuvteftd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rzwxfbhm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ojmtnxli.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hinlbdyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giasdwrg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qvkbaprd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecstsucq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qvmwauqm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lrghzdjp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3plfscofs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3alttgoxp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3awuusqin.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3owmoegxt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jvwnlfjn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3otzywnri.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lcsqijwv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3plgbugam.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dikecmju.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tapgmwle.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxshjcm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3orovksak.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3redvehaq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yyrzronx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bgncmfjy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3smnredlj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mrwtggpi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tzfwopir.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kzqqdkzf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vscdcvvx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jjxlaqca.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sjerskcy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cffefahq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3leeovbyv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3slmgdggz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hfcgnwty.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ynezizhd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jpxdvosm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kwrosvbk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yknttywr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wrgscjty.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3idkveomj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqzblczy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ggnlhtcm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pwjbxuga.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ytwicpcy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqmdwsay.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3koguxwxc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3roaisrsm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iunonsxj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pujsdixk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xjbtlugc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wtxfuvtb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3drkxddxl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ksrybrjw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3leghkupn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uwupsngf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mawtfvkd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pxgvsrdb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wjeilgxt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkanby.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xzmrgsbs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lbqjkgyb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3oeihvkdn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lewyorjt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3uurrpbza.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zfkjqbse.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3iofumyog.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qpynlhmi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3krsrrovs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ebpgljtm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jztlagjp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3agwkdguz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ctueeevy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjuwyaiu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hynhlcpe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3btkkswll.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hvphvikn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jrvmeroe.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jdimrrpm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3arcufvkw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nqmjxbhe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xpftlfyg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zhcrnvao.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wussrlbo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3nfqjbdde.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzizdkfu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mbrsshuz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nkiopmum.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3celdzwsw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bsquipeg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3avbomzyh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yxmxrmcn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3orzfbyvl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bufmkuez.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vghikydt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xbzsnpyq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aycfykxa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xhbfaias.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3snzqsyon.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3okzztqna.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rowiwhdu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gczoutgh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kvolvzlm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dqjdlgmz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojxksyqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvqskupk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3htteeexs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3exmcpiys.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3klfuttju.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wcddxkzj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ohresbqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ypyeeomk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bgseknof.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mipbtlkp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rpglclsb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cbybxjba.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ykfhrgui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3auzpaxho.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3boemkygc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nrgieepu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3opigcclv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3swvkhfab.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mxhlalwh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qpfviorq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3acgmddnp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3igslarrw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghrznkvm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gnlxhnwn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mrwuoiog.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fwmgjioa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qoduvfsh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ofvwysmi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ltwishia.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uiaeobkd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgwahxyk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3napsmmpl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jxwatvbd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jtvwdxio.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lsnryzyp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pmdsmfqj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fhcxtdty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bgzonsoe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mcmtseej.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bhfzfwge.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qbzmtdad.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3arrbsmrv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qgkqjrli.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3miqlfxhp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cibaghdb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pwpttqqc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ufqbtbyu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zdfjuzht.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hgtdbtdj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3anxsxjvz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3giucredk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqjmiavq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vauhadgy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3toehalig.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ueioacpg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3juqtezwi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3eojzgcjt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wyicetzg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rqiohixz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tyryezoj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qzsquayh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pzcsgbbz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3swsiozmf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wpfexzfg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wuatowfh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvbbujzy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mytvtjwv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ogmdbsmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idyjpwvk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bldcvjwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwhrlgjk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ppjnjegc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ajyvoigs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wihbqiqv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mbtsfgwf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cqmdjmed.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3soxjsnhd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3doalgbwg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gkqffjwk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3giwdurkv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nvhivake.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqcwwbxn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nidelfff.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yzjnujpq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lddfxftt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yozwuskw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sgcpcqzi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sjyjhgaj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3unnlalrp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ltfffjlh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3klzkiiwh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3knybfrtw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lhplxquc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jqhnvvlw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nqukesdj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rvcqvvti.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ggttsvwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qxpmvtcb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3atkubhgh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fhxhyyov.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bznbrdgp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jwhragob.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gomzptpj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oextasyx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pxpzwpti.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmjmlie.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3majwghgc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ixfnacqk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jgjnaiib.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ovsdqqqz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tikgevkg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mltkwkti.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3swsumedz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qvnliglf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bdnvcpyw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3awknawqr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3brvihksd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jrmalnpc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3utksixua.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pztnnhvt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jmxxyfhc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nteefxzj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dxjkkixc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3riiducsl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qixqifnd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mhyxkgns.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ulrkyawt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nefrmibt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hpqiqboj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fvbwaxqj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3znnrqxwn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bniluhda.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ftzoukts.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3brsmdqgr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3uitwupjc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tcbvujhm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kkvyahgv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ndtxrmrm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxwsbaid.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbnqjzke.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ykgxxlij.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tlqpcqfs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3psldwvax.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3sfkbkfms.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fjpllsos.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3boukoaot.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlnnrydo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3aarrmmrc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pdgicuri.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3eyjyzdcj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlwlrdvt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wmvklcgr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3celtpbpo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jdfitacd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3poxkjmsx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mraaklaa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cecrgytx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dsxhvzur.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jmminpar.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qrnqbwdr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qcvvzkkn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pvuggnbb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xivotovi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3aekzmtji.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcjllphu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ysfpgwuk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3devgtbxi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3umvhxpye.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3okgsmani.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tbyvdqzi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nagmhpya.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebjynuce.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ceqxwnsr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzfjzqm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptjotypw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xifkdtes.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gfvdnhlr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3okdfyvmt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdyqcytt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gbugwxpz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dhuehnec.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xkpvhago.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3flrcgjdu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mnldekuv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xkqdmtpz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tbedlroz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kudazrau.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmcxktfb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3iymicquz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrisyoxx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mdekphid.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ssavgfyv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ktieunix.html


<!-- 参考信息 -->