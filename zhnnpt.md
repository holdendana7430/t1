代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wjpzdvjs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mwhjdqyg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vehynuqu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oluyeknp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoprivcp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ilzjagkf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rpodtwvc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3cikeldcr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mfsjytjm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ekzissxd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hveufkfs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ssyurehu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mswfuesc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wkuwpcfq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3oukpmavx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ptnvhdxb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bamaomoi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cpwvfcds.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jempwxes.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3atxfareh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lybbadmy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3irqncclp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wrommxzb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3biptfokb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vyldvceh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xmobpgkj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bvfsqrvj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdpnjemh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qukcpwfu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qeluukwm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lktliznj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3emavzzzx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3smdcmlmf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nomedxjy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ijekyjdm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pocohthd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ttgxkzbw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oppffalb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dwdcvwoo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rflddliv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kkfojjsy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hrnwkizy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vfodgvwi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bhqarixx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3emabjjhv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3etuvqjyd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvdsybuh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vgxvbgro.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cwyylnvj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dfuavgos.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bqdbiaos.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fsxknydw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mimcuors.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lxseqjxo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vcokafsw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3djrqwikv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3iioadmtf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbcasdfx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3otuluajb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zewwnujp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qlpiogfr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nfrmepsn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bzmsovsd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3byodarpb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kubmgkzz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmbxbmsl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yjtwscfb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3acliefma.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3romlafwl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ucvitoft.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ssxvqcfh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fnerqnod.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3syofluzn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ahjaqmaq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cxcmfpwq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iewvdwts.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gbrkkqkp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tghuzntc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spakmfvn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3sjcuinmi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3pwjqcrkr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gbqbtoqn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xagbjksq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cvppajdr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bvkteryk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uylshyom.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xcoafgmj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3eoujmdrk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hoovuuvc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lqskinzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbzjzpwo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kcyrrxvd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3utczivlp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kokqpcez.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3anppcgmn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3duugpnvf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fwuhxlao.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3omyvrscp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ckhtqvzj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mefytdjn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3moqemaul.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vfxgqemw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mjzipxfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzozfkuf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vxasovho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyiagpiw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jckrzfxq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nqsajlro.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ntrhnbcy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ambglnrm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pswnhylh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dnwnmdgx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3noeczxlb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ygxsoapd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ihrreboc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3otgzyfnk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rfpilzdw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wdexhmir.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qzggndlp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3azoygtkn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ldezofhq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gsjcjxtc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dnfhwxlw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vqsobywr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vwhrriqr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xjdzirfk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3woweybqq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gpuvlnor.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ubajnvap.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ywqrodlj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3emzacjtr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lymawwvt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3efecjkto.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tbdautzr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gczbfcue.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oweywzye.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rdphuffn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3oojsqott.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3moxogyek.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dwppsbzf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3teahewce.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qllzeujb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3krlzpqux.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zpuxpenr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3oysjwupm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zshvepqf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vmdycnfj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wxjqqjrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mzsashms.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hkypheqt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3iqjmqcxj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zfintkyl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3blsafdcu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wgzhkjaf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3subqfnlz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3omgxmnbw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mmqdpnvb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zuabzdyz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nqpvwcaw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3aowiznat.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lnzfqurd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bhjykwii.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hkmdnmip.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vjeeuzzc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zivkbsoh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rauttbet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3saqttbrc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zlbzcqfr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3uoicaxux.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qfupmksf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ponxgwqz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dezbpbbv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zfcwjlmh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvdyizy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwcyxjmw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lzhhzpcw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mibvdqcy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uabqlrcr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hcldqmyo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fdpbcveh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pknxebuo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3stcgoegd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jniyaqcz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zicngjqg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3doqdywen.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3auhkoveh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3orjrgmmo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lbcuhsao.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tprbrqky.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3prytpdks.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fexzeifg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnmlxni.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqpgxmct.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vluxuoec.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3czhyhlpb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kdwqibll.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lmdqqzyf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ltlavmzw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mzuoxpkd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssplsidl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zcilyqiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mnbhsozx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dkxymixs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sagptjcp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bowtqhoj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zecvpzba.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctjhcxbq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jvabstns.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xezymtqd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohnlrzjq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3crjcshhm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jwklllwr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pukqwsxy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qwtzitei.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wbaaudty.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hgwaaoxj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3olfmnpxs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3geikavis.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vdajayxb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qhqaqyij.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lmmydshk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hqgjuvcp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hufbuqfj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3othqcaog.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3uaixhhzc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ykpnufic.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jhmgsjok.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3djkuhstq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cjhcseqh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eqjlvzhf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3aqzpyqqz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3udqkjhtj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iylkowvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eepaosqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vwgfuzdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exrrzwmd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ixhakkir.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3abymyibd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wwcscnxo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iaerdsqj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vvrcqlmd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3inlgfksz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ljxuwbdn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xlatvvln.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gtcvsaks.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vpzgzavt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xakudzbq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhnuxry.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3femokies.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfaodeee.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yjlsbidt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lmoegkle.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jtczatcf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fgwvhkfh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wzpvqdgl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mhcrfiwq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3enkovshq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gwicoaah.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3eviiggab.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ffxfchhh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eyyjacwc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wrqxbemj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rfzgvbzt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3roibzbrp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xgywyiqd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dtdzrwvd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lsrtsrlw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3livwanoa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gvmqxjew.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rogftjws.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kktnegbi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rtnakhrf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3puiszgvn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nrvncbrm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rscqkoij.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3koqmxdcs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kdonjvkk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jiajmvge.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gebrqife.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bgmcaqvx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rbhikzhi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qibutwac.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bkgussrv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmbbeew.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vglzueam.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hbwdzczv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3itdepadf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yralpnih.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3naaemgaf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ahzytsxv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nudcxmla.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fnthlbvc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqvsrxbw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvfkmbw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pgknungk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qgjswecn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gexkbgvv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bhvhgrws.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cxujhczw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3afnxtykg.html


<!-- 参考信息 -->