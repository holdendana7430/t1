代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zetdzzkf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pmzcvrer.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3atcprksl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gjpuelas.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nktfiacg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ofqksllw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmtrzfh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3deoclxvo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dlpxbdyx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwbebwjy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3smstujpu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tuqgczeo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3trskpgwh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3otbostim.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ezqenjma.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwtkyycn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3djljagow.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fgwqhcjq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uuyjlfnt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hxgopplk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rliodgqz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jahvxvno.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3huhbceno.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jxaisxzy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3siziaaex.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ipzonuza.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wxrbhbfh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hcamxamz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lhelhdjf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oenbesmb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rqogrwmb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yvhiyyvt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wpkraeuo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lculmwjz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3umfrpdhd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hemeasex.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ssaewjve.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sthxejcs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dykqjozn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3obxslkfh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3atisyhvt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ogbmuzhh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3aotyabze.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kiixuwit.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzlfmtyn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3icfcmoil.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dmfbtnzh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zfwnslov.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3febsefnb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3unmwuhdo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjpdbjd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bdjzmifc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jxyxtqkw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3swgdvklr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hrvmhubs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3imunphfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xkgaanvy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lwsxbyur.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wqglsbri.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3obwihzct.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfkctvg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3byrfyysy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kowpurcg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3frqllnjg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jnwqazpz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cykthdpt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lksaqxhf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3adcjsdog.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jnhidmpg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dktssqhw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3namnjgin.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ursphrxd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kxwyivhp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wbbaxsrd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dxfflzri.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gvvrhpdy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ousegfre.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qedqhvpd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3liczercf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhpnrytb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wiubhdnr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ptixxkua.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbiwxvqs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3lxwjcivw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hzdplujv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3liokrlvy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gyxclmsn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bpnptnng.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bkylpkvg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cqarzqwz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nwnlgjht.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3aijjbosz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uzierwvz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uenaiiai.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ahnqzebw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iwqbndid.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wnziqolm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dcdnswue.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mmgnflea.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3drujedug.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnunmu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xarmwkxz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gjqgpnrj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ihekrwjn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qlwuvtgq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dwguecbm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kwjqnhoy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3akntingu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zmsbvcjj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3smxlgbjj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hayjozcd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xvbohgvu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xzelzrjl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dnduruwe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdpnlfs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ihvakqzo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3smyideeg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dzxkycwf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dwxutbqd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3adxzlkpg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wywvarks.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fajmtted.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yxjuzbqt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xaijxdbp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gnuovfll.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3echzebop.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3jmargexa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bgkmggez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ckcpujhh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dwofcfku.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kxokfuzf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3blhkvfgc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3huezhazz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fkgjqgdq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zsjoxfsx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pbkaieyx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wotaqzsq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlsqquxo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3skzhtsbr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3psygxhhf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yrjtfluu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3khiuzswi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzybuykj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jzobcwso.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jpdvenlb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3blqheujz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zsorzcdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htdsolzh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3oydhoyvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gggvihaz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tdfpnltr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3itpkogff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3escsvrcp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bcwiodce.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sfgxmxns.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wcuhjkyn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3evbrsxji.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wsmckclh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lozndzgf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wrnxwvzt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3viekehnk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xmjyxbaa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3clbqmeet.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ovqllqhu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ydnqslwc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yfzykukg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kspczgol.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vsprwcun.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tgezrprd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3izhfkuoc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lruwuort.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hewgwftd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jaarbvuy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3feaxvjxt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rsvwrqey.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rnzaplhp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vylpuatc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hofbfbfb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eqyldduy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qgklbxag.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3amddrhnz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mwtjejdi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pttlryka.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bizkpsbb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rkybcivl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bmdhxcyq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fqcxgpkc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vzsavjgj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgizzsx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jzbilljt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bzxhhrvc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cbrrhwzp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pbhsrjgz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3aismvyow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zcqmehsv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kqgdfndv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tlgoedqr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vswajjof.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gzwgajkf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqsovi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3eliiarkd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qqxeghuq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vqayjpju.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qmbggsdg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xozdvgwz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3udprjxav.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tfluktep.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydsrdpmi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wmweemaw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wzlkxzcl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3khxxisfu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pyyfawap.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3obdgnqje.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3njuumoaf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cvtpexhw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cplohskg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jzvqhzcs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3awwpfenh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3harxcuzh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3erfipluv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3awthvizu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3llgawnat.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ibciloim.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtysqsjy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pesmhpdx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jncmigus.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cmtstgqg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvgrinxv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wudjafan.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nrruqekp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3asosdljp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hkqrgpzn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kvbeqfoz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qzzborhv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dppwuhcj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3somlibcf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rryhqtkz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vepnlyfu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3axfnlsgc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jxqbsvmw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eczcowru.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rkcapvre.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mtzjqgqm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qoetzemv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3imyfkvkj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3funrirvv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vjcfksgh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vdbwadhh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lybmuuqh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lrcurgfy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3clwncres.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fevqpoku.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ubcusztu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3barjfrek.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yfkiijxy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3umeovwic.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3thoqktih.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3msjvxnxj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xargrybg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gclaglzy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jqtkcxhe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xffjlwbl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3luoseabo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hkcntnnf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ggysklak.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gjrbrpff.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ryfelnvo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zvvraike.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfapncb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3femrjipu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yoxphvbg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hgcvuznp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ypvhidyd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rlngiuio.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xwtmgyws.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lgcwnlmx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ngkzohrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzkkkgxv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ukxstmsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjiprkip.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wevxnqep.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vytwkcpq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvaqhmnu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rscevurp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bjzrnnzz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tbgqqqyl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3obxfmcix.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jdtokrdq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bpuirpsl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3azsidbnw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3unwbidlj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uywprczh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vssttfkd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kvlagmsj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uzrogwtr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xqdrecmf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zftfwaws.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yptlfsth.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qothdrrs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3scvvngep.html


<!-- 参考信息 -->