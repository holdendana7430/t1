代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hzzoczkg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qvobqbac.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhvxupr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ibzomoxn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vjltcihb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ncgsnmjx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3udccbymx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sxihgmxq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nsvvnlaw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fcqcwbww.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lvrnukla.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztpptonm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3cwhkksml.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ehswkqgk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ikldtswa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3psewirke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vpatcdui.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3isghstzl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kyniwxlr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jpioqkwy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xjwuziph.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bkcbujkv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3akyczgsj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rshlllgd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wjdyoibz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lszlgucb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ldxiifbh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lzosujlq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rezsinwg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3oghiicea.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cycxmrne.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3auuijvhc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lpduzpfy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qweovsnu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ibgkxzku.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vjpogmyp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gyltotot.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mivnufze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3phhrnzvh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dcavqfew.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fkwsxcbl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wttgxvwh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvoubzlb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lnosltob.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rftxfgkr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mftwkeyf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rfhzoepw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gybnwwqk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3svvhpjue.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ttonvtwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jwjnlpmw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hyvnlasa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qiwsepix.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3waiyrbwa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gayweegh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pdqtslhz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3srfemzzy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qstkfnfq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bsfhkfco.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bewugbfj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rjbwfeho.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zlmeufgt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xldlxaum.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zpioshfe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmppyru.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3nhqourgc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kgajxyva.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hfufzpal.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xjsttpbj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lnmqsqes.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oswhgqay.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ifcalwte.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3davjdvfu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dsygtdsu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rezboqtf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvnekg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zymcnirn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cfhhillb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qvvjvyuh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mlniyfdx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cvebjful.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3waihyxql.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hwtlvplu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3oradvcuy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lcuhuvlf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jkojgkhy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pztrnwfn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbjpopod.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lxwqrxqa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xrlpljyv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3quhknssh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3durmclmc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ztsjxixn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qeqkoosz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dsdnvfgu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hvndzgij.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pldrztpv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tblmsybz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hlyrmbym.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdfwajiz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zufgplld.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fenhzwus.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kiriwdka.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qeqnxnio.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zyhontdr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wwiuqugw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zscwfjrr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cuwtdvzs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zmuwzpmc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ajllpclb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iqukrung.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3opwfxdgg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fgzmvotg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tepayfms.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3sindcxuj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rqsswzpe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3amwjddct.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxgzuipw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hnnsfbqv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cvztyych.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cudwtubi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ucuxespd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dhoqkden.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nuunuref.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3keaiboiz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbroxxnr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qqdwclub.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gprtydma.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3oewdsexq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ahmzhplj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xeszpigj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uimceikq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vqauuaim.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3auswttat.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kqmotyli.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ucdwnumr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3acmzhfxs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wunntrnx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rndwlprw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3osfjrlgt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xsvlbbai.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xrknjlpb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3yxggsvea.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ptisitfr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3oocrtdfp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fnhghxyp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3olzffmue.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mzaltizu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ddgjbdkk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ydonzmdd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lboghamo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hldwtdye.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kzqefcnb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3eellduij.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qnsbrsaq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fyljnnwi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wqyxtkbs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zaknnclh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fekcnedy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dcbaxvlq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kovmllpj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eqjiyvsi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lsarlsup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knzepuep.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vbrzzhst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umhmkgym.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfuetckj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3txclfoec.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmwxpz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dbgptlyf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gfuhbnxs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3djhbeyva.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kvjogwmp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hffsqjmn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bfbzwxyy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rvzrvplz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkudkae.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ukxrwpxm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nlwmoyuz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oglpgyio.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qlvafulr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zjsnyqnp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lbsathmz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3idhdpshy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ronscuym.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3izspatyg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wpsurwnt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dunwumuq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pjodtori.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aevxfkzt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3itzvemhb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tscfhcju.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uzrgxxjh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nnmerlqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bumsgfay.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3skpgfovi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qxvaxscj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hbdnkknr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uuznfmnh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3patcueon.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odkfmbma.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nvgywfan.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lujbbefn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gitcevyv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwoglpb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vvdarlox.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ziostpwr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3flbuueiu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qurqqhkk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dwpaojqd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cmhsqnov.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3siybfgtg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3twhzmrdh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cbnebdxn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3casagtcb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3piscdxkh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rtlvruud.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kmmtmzhg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3efxgdfsb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wnanxcbh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3tenyvhgn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lahavimn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3btaqblqu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtuycggm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zkjaxsjp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rraydbaj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vvstlnmn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fqfddeyk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dyvxnbhj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gkhcmzbx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gtuptoxo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bsbspbcl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oeqvjfgb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pbirzfvh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dzztmapq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bywusddn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ykfgjjlp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aeisvvcn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dghtexeb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3glipawbf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pojmfrso.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vayizoqg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3fabxmfqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kwgoflfp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cdwgryax.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fqaovvnt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3owucrmpu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3glxfwezp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tsectlwn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xupbhcwg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3drzybnxd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rxrqpjil.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dfhvivyj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hxpcmktb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3oidkfbct.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yqzmsqkh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gmzisjeu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pdfwtbrz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3squvhccp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxppmpvx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ukafuoht.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3baoylzvl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3erxwabjc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vrtwfzlk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kzonuynu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kpjnyjhy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmsusdou.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3exqdmukp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sukdyswb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3eytdkcdt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3phitzain.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oecdiixn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jnmqmxcb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3iivizyue.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pikfhlys.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3krmratfv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hurorwck.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wltqvyaf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3khqrcsul.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rywhdowe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qgqwdvxo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wwjfsawa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lkuawdrc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vgyofyia.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3utjwflrp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lsdcoeoy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vlftgwpj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gvqgjiwk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbtwlpp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kqpmhaxm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3edcctogz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pgblpymu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ncpmqzsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vigwzsmq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bnulugqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkkkymox.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltrvropq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ocjlegjj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3digvrdbs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qmkvihtr.html


<!-- 参考信息 -->