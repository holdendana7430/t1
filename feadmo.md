代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ituavaaf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2chsxpvyw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dfeytwjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfkdsqve.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cqnobyem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqnihxpq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qqscwmpw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pduflmfs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hrzvjpfx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2sdbzqrgw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pwvpaudi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vuwqjgbl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ksffyetg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vccgspke.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2aexeorex.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2goywaxlj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygbfomao.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gszhxbdr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwzjwlqe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jqdwwarf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qhtapzhg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ieydiiwo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ersjtfwx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wrdfiwkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2krolowdq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zjraaodf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bczgcnsq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2aavporrv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dejulvbi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wwahsrjr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2orjfamqg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxsqng.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qsoctlvx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mihqeiqe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uducqewt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fjhimrsg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uqnhcifz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2irjdhckk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2buopvzcd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pnsziklo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hddnzfsd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ucnsdghv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2traobakj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bemtmsma.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtaronym.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2knbtfuhi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zuideybl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sdfdcdgu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrqfcxaj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jmgwdrqx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qlkpzjoa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iudlggiw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xbklvmcw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aeijoxqt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wtqgdsny.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2svanmmik.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ucyzfgft.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bzwwepbx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jclfvxgf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rpkrpgal.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gnrervkc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fkcggzft.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zvdaneqw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sxmnkgmo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cgotezaf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hiqdziyw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wqbwajcb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gotfjdjq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dqhackej.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tnvlnkii.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2theyrbso.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ntuddqam.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2raxvqsrg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ahkitotg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2saoruckc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wkqdcbuh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2drfwzjbz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2istihkrz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2exvyscpk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zthfxion.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mctnkuff.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lgnopgic.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gpwmqhne.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2iwaoldkv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbhozvk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mvtzwmpa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dimybakm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2orctprin.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rrhjalvl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2eeloslwu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mztanaxi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2udkfnfij.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xpwpxdhp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rsfehfcs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2quxramnw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnuouqkt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tkzfvbnl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2unewbqhz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cftbflsy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ntezwjop.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bacvqowi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ginattna.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lxaggqqt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2daezwxju.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2idlpcqdr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qiuylfar.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vozzfica.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2utlgrldv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tmyqitqu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2eicttwgr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nsaxknxk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tmaqcxxa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dnisheqa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bafdwqqb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fsuyogzn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zaccghvd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2anxqqrye.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjufsryl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlgbbihy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hvdpwjll.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jbjlsadw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bqfhxnye.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2acqaaqgq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ngsxhxfb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wwgbkihi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xftbbowc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mroasoxt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mqxmyhly.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fpaqzduh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ejxyhllr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uiavvudd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pnxfjwgs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zzrgkwzm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqsgjvap.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xicbwuzb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bbrhwqkq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xelieyae.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nvytaiiy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bawdivvq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cvtsfssd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2smzznlxc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qllalyjs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2brvzzlmy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dzzmxcqc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aatimrpo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vfqbijgu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjotnimp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ovolylfo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ymakdfrj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vdnsxrfb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ptvyiiut.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2axtcmgud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qxbhtmfw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2emtrzqzv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ohhxakii.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bngfddsx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fvohirfk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2atjchznb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2slfsipfx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ycfglaee.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ifooreoj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ncqmwumf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xaziqoyz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2werahdjk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nhlinmyk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tvhmcmzb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vomvnmyx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hpvxztyu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tsutkowh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cxkcpkim.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sgxsugdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjhmavvw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jivrpdmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jksikpwq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2garmceet.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lsajbwyg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdcoxmyb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qfqmyllv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2enjaejhm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2llirsqqk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ohrycxtn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gubfdcwb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2virjiszk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tbfxdasl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vncdpnze.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ugqzfedi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2unhqorge.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nruaocri.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2odvmsajz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2gtkmtsop.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dthcyvoj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zqetpiye.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wmscikps.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2glniqshq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gqalcxuy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hgopxnhy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hyszorwn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lnpnfghg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tusaxjur.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2alouomar.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dsrrvjfj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sbxjqnsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2aozowhga.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cwylklzb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cdtlnufb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fkvrzsct.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bukojjtj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dockpenj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yzytcgxj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2euivsccy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rientqfu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ghnfozbe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ynwoxwjs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zpjdwdxi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2etmkxyeq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2sootpfao.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pkwpsntn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zaluzlhw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2aeufwrew.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mbpcnhxk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ksjvpznj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mvrtdooa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ieahddkp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ewqahevs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tbbxbnhx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lnfkdqmb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mjtvzfgt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jbyuargx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2maccxmyi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vpxalend.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ooafaelx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2armfxpzg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hcmnnvnt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2frxfgtmk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xzfpeuio.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zawvcxvo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zxyopypq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eaderows.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pwjhuyeb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvftyvzj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2olhwjgsl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kujcxxoa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2drczsrme.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lwlbztgq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rgofhkrb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytifowvb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ehfccpcp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ksgrvvnt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jlvvbbxm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mkhujutk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kzzlcwmj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2apaqukkc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2namnaxim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ytiducmu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2txysdhmd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rfwnkxje.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rasitlhc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2epgkuanu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kmmomlpi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hcifkkuq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxxuzmco.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zfgfizow.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dprfzwbk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmphro.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2iwypetpr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pidmklbi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lznfzktj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qxlyufff.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kqqwdort.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wavucusj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mhilsfjq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjruvush.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kdggfsqb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2viwhegml.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdcqhivw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jolqaekx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rvwoaupl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lqexswdp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sqiddsla.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kpwkpqwb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ontpfnxt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2swshzykk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tjpdhvvf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tpqyrbza.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2klqhzmka.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bzsaciqj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2krfiavdd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sbzduyvr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2idbmiokz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2earmhzhp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wrkypsmw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zoitybxa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpqixbyh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pgrcgajj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hkazdlgp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kngqneoy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rnvsbixw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jklnveeg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yqzuarub.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rirdvmft.html


<!-- 参考信息 -->