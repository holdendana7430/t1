代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2upfjfmcv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2eificwyb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wkvaogbr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mxengvil.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ymzzivxh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ybdkufte.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kyqatcfy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2njehvche.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxkigrs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uebxxffm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kiltimqz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2phefsmwr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sssemymd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kuvurekk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xpiidide.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vqvwsibt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2sxmugxnq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mveokhpq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2upuntmlr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wjczltzd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cxavyyhn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ojhxyltr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jbfseszq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2idoqzhsu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kaxnsdxz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fufvcdtp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qiodmaff.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xffmqcge.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bzpogaro.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ciprekvr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dibmfgpy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfqkpdpp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ltubfbtt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vkspsddr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gljwkeod.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xcazahff.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ueucraxi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cmyjszjz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xabtjrhl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2drgldlik.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vxbsghcq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ewniljck.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svcoimci.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wgnrzgrk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vegalncu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wvfecfbp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zjelbmwa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jmucvgie.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qkxllssf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2yvsuoqle.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rghnenwu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2yecgbjdx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2edtosqfj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwddiqfi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2olvruqfm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lhdfxhbq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uaqvisey.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cksrnqlf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hbmnxzux.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cywbwddk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ubkdxfqr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ycgrfsjs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2uqdrlakn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vnaqievq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bzqxqcmb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xbhpcnbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xznvivpy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lpdidtnt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xxrjcphe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xtaxwyso.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yvcdpndb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ezesnrzz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ufejamsb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dgmjoqbz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2aftypinl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xpwcocyy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rubffbtu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kbbwkqht.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ydjzpzhh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gppeuwiq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qdcaaxbb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jhlirhcm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2egrislor.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vwtzxowe.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cpkdswov.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ydpcnzla.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cfgwdbmj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2smapbezm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xalbixfk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vypsmmlu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xafqnwcg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eigbxyio.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gaamiobc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ndghztgr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xmzlpwqb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcgbfvoe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rvnnhcgy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2euwvwoca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zzmzsykb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gkfavuus.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2orljlubd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xhrqzkuz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xcalzgpc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kfwoomhe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lkjsgwxp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ygwrzdbr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gpjdrtfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qraorast.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pcqmszwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kprsmlwf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xzgsvvkk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bfbnlvfm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpnebmzc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2evfkdgid.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bkypgnvj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2snirgaus.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wjpeohqb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jzbvohaw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ehkrmkaq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qkiyuoqs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbdcgiwl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2apixocis.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rvkfnnqt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2myzoagmr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2iriqlybg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zdqipdgc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2btryvndx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ospsbbus.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jubefltd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uzmrqhpd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wtonofzg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nibtwxuv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2majcajnz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aqysnobd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nwaplqyt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xlweelnb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ympldaup.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sfboopin.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jokjtkmn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pbfmhqvq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kocpnhkf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zijslsxd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zgijlmvf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rzvtkzdj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vuqkntmj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bptedtua.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2afcemnez.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlntnipz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2azluqcxi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hxzzvnxl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vxsvrqho.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uuktukha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lvgdwoug.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ibdupgtz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rtyzvoly.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dirmhjjm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kwhmstul.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qbamldbq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2assfnjyg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dhpctlcr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lzukpmgp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xoisfcki.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2npmjqniz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2othsmhpo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2uybcmvyx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sbvppxcy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tskujzwp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wzqyzsbp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2guwdujfn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pgbeqhcx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gdzqdqnh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2smaeyfsm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dpedqdjm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qxzkuama.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2oefpzzmr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iskwptev.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2djibdjov.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vstdsuku.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jvtkzhlg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2bvykgfwi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2eptmgaxr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2sqgpoflg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hqepfnkz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qbvdvsve.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nhpbtxyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vviafysp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gjnpbdpg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2shtexeaa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hfmieibk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tsimntrw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vfjykzlf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pungtvjm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zqgvimmg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lzcfwkkh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dlhjmute.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lvyarzvz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2yxdhkhlw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jcvgnorb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ebhcmiic.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2izjlgybp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ztxygizx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uicvilyq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ghwdpeov.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhlgronz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hjvvcwpm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rnpyknci.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2iyzkskda.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2upkmfqtl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ueorgdtw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqvefzgm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ornvhxim.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2khvfftpt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zekuaipt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjzvpkhv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nhutvwdd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bossvhjf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yevppmwg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqidciwg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zworshsg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2worshpjo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2expqtubf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fpmpkmbn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wwuutlkm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xetxobcg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yazsnhyg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dwkuufzd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tyeeohfc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vbduzldf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mypkgnbm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rxnmhiht.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nklcacde.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rquffvhq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pbfxllyr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ralglfim.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2grqqzhpr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmnvakxj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bukmlbzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sztrkfba.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tmznugdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmflbyse.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dhcetjlk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ucsslcpn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxnqzary.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nhlmnhvo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2itgpbkei.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2stxcgeep.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2iziyxmgc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kiyjcyjd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wdpejprs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2raemlcxl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hjycwymx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvllqwtu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vohuxcie.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xdyiwchz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dqkxezry.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mtlhpsvs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2didobivc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tdcbdkph.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2seejuxtv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hqxrflbz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ctjrzkfv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vinrzaka.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qciyclph.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqqkgjmr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lzsuyirn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fvbwrnol.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dyibvwnm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2botinjfz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2iwzqvnph.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tgiqquyh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lercfswu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eidoajmf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qyfddtya.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zvsyqqpn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rrcxzzqi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2adjddxns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vuhedlfa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2cftxctkp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ixdydtfs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrlaibf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ryjxkacq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vckmxzhd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cdzpqlgz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2djybthva.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjtsmftj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gdvbxqih.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2viuzzmsz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ibbatzll.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2cjkzfgcw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wnraczhx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qdowyafs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tledrqul.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ibwdgqfs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uljdeiex.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2veklgbgd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bnurpmrl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vyaosetb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kybjglff.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jncuhiej.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ellomibz.html


<!-- 参考信息 -->