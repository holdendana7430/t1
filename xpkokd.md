代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcnuewum.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eirvsavy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cevvtrzx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nwpunsxt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrebgu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fvpttfsp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rxtngkgd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jefdnxrd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tfhyjohy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cdldykcp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ydcnddup.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jyglzfsi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hlfbaobn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rhwsiovg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ztethxww.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lprzbptd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zvmkzatx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ggvgzqsr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ooozvaex.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dmalkocd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tkiezyvg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qguihvrt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3myesnqgn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zqbaicpn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nkbcmfkk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3avtmillf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xvkprqnj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvgcjnuj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cdukyonf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3syrkhspi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hwmfvbnr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zfgkcqer.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dwmsthqd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ysbxcnok.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zugmbogc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3itqjevrl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbdgfcej.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uctjuuci.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nongwqhu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hyuegtic.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ilpjxwxo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3oaazlmfe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rlzszeuw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uulcfdoj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pdahztus.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3etcoavxu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfnvoaya.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ashjpwfw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fjhxmwja.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3cabavgqc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxvjkevd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yrlienbq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bbtfftrx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wyghbbzv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kevvybsz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3iyzwqsuz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gnrbcbbm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fenzakmp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ppobcfkb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oxgdbgse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vhgfonxe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ymtqgryi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vnmxtlom.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3atxieayy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3iaepymry.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yhqnhgsa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nndmiiek.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ljuiuwdg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fpafndae.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ahslozxt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xfqpkrtu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3enhxierh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bfrwjama.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bewjrksg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3azdxmrfx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3alqfiqph.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xckbnnux.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lsinnrqh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrbfrrgr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xgfvauui.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mltysaat.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fnafwguv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kpumsvao.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cyvyljsi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qnfteaii.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zwngsqoy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rbmucjms.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3frvsxchj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3urlyfynq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3afjgbufn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dyddpqde.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kdicasco.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vtyivgcz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3fxfthwqu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3csdjdufs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3odfmjknr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3whylzzkv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3uzksvwco.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uvvykxze.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gsqwbuet.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3huojnyjl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qleysoto.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fzjlhznq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3diwjqyir.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jccoflmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuxnxyls.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ktgntjxw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ehyowmxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yhxxgucv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yjefafbq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pmxaafdb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mqkrrmnn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rgnljowy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vplmdpep.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3smzgqagh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3toigcuco.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xytynfog.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mlgirpzw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ozdkaqeh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kufhjsgo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xyczvnoq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sykdexsv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dwxsbwtb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3eieafnnw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3quhkltsm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hecgkbfn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nctmpugy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvzqbbwp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ieupbqul.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uxnfubtt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ltdvelnr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ycsnminj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qnebulvg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fhuqdzuz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3frtzefzk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wghrofxx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jjdbqmyr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zowymirs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jslscbeu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jkznlook.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3awyrkvbw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vgaxyslf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rfvrschc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bzkjnahq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3oijwzwnq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pvbvgwer.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gbwbyeuf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mbcefgsl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3arrsljos.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ehgnvwih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xfgsdnii.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fpexoqdr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3idkjtbzc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zxskmcuq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vzdevcfn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3htqiuuvz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3eohsxsze.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vlizkmfa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3frknbvvf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cpsmkqie.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yjjabjzj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3odwcglwh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3abcvbzvq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rhwsyzdx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kcimtlwm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3aklxiayr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jaeznhbb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xgegxrxg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3biyxaehw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vylheszm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xxbdvrem.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xenyqdzf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dvecmkeb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3iqepqeqn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lrxmgygn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xhdtsbcv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ghpnqzkk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3govdvvqz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3feipryjp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fosiuhaj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rcjvbuzu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3teobefrj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rgxyyjwe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pobspfkg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uberheei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfblkhnv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3txgvpyei.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lammxhvf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vacamtgb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3malofgli.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cxavksmw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uzrhzjpv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtafopwr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3enegpwnf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwttfwsd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gfnyhlxd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pfzhexdh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iaildwqe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vwdtsksv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lcjjtmtv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hsvzzwpw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3sqdmcdey.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zsvzogey.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3taxjgbof.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3baxjiweu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckpowqzj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3isxbzrfd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qbxbghjq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uupjlbrn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3toeankfr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jedibmnt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bgixwmrb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yevgedow.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gnqxtiuh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3susvsaqk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ltfyabns.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wcqmimkj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rcpaxhqc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ondpfhus.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nxainulj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gpkafqeo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zhprpjmd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hkvxwiui.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ktmczwxr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsrsydgy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vzaqbbfz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aggmkqgv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yubtozev.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zseaizkd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bnyoxopn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3pwuyewxl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ksblkhub.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3idhschsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jodkuzar.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hbuafsgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htyywgro.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zrzwncpw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ytexbjfh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3reseubps.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3grxjtvmh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ovhopkpy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dculfgud.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ywaskopb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qmghjbfp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yufbioop.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xoxbjzds.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lzqhnmwg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qruxvett.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pqjkijgw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ybwnxhjp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wclwazqr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oasmylgy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qtdvvsqy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mjqiviqc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cknripyf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zbweogmi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ohraduok.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hnscgibu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ximntqpt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktelxoaq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dpqkbfci.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmqcytbq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tjkflfmy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcwnmmn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pyvmwewy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yubprvpr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kutlrsrv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gyqeoxop.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3coxmismq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3meradxpt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zlksxnsv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wmbwuzna.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hubotkfa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hguedeow.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cdolhklr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3swsjkdnf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3obvtqiqg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytlsffda.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3orzdsfvj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bswgkisl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fsetjbvf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fzrwftyd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3sjpyqfcs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ogltrrdn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3muczkzjm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wiaeuuca.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uaadpygw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3klhocnsv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kintvpuh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjwahjou.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzjesbte.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rhopklsp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xtyaatwm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ckbrgqfi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zwvvlhew.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3puzyifeu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cxkdvdna.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3odsqcvfz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jtywbekm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vadwavag.html


<!-- 参考信息 -->