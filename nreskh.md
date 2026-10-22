代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ggssujgv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sguizxhf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jugbgnlb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hjuvdzzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2esxhdgyq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ngwmwrhn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wswqzlsb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cduvknij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ebcxkdes.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nufwuhvo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dpajxwss.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2eeynohjx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vhrysryd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mfbjxoyr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qwieoigw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zsnimbxx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aaksnyfk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hfyzsndv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hexeyxrm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jgpybhhn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bgtkboij.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tkhcahhp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cqnfpglp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sgpmidmk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jbzoxrxx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cmvvafol.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2otijeqqn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rlosmgkj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pgmyipyo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vnbeksyb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lsqugger.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zkuzenhl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cckpvkjy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cjlfgxfc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2glvgmyft.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hgmrzdep.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rlrbaudh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lmqarjyf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ilufqwav.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2prznzyqj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yyqhucnj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ccrcmxzz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rehflsbt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2likdswhc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nhabdjuh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jflhhbnq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqbalx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xbzdxlpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2imcvwqhc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2raioviyk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rekfmlzs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2caukwkhq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dplzaabl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gjcitchi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2obylqcni.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kuoqavlb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2aneszvtt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mqgiasnb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vbonzfkp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lsrlhcum.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wpkouukq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jaxckdga.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2oabityzo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2gmaweqau.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pzqslssx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2obdqurly.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yrrqlohm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qukuaxmo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fgtvzmya.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kjfcervg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2owgfejei.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hrhvgkrs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tjeakzyy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zbuijjuy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fevmkjbh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wyjdtzju.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xfkfsiwg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tmnabcsl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ynlwwsve.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2thzlqwzf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2glzymzao.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cegusrjf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zsgfwruu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jgdrwdin.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ippzwnqp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vlbyalht.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fgoucnov.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2weszuums.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dokitabz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpdojohh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qwsbaekq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rygabynj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2grcnwhdq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mwelcfku.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpjogmpp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aaznhmsl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2cyliwxxp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cteifwxp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wwrrldlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chxawnlb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cvamiswu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzdbhpzf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iwitfboy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oolwxoxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xzqzkyum.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vtoxjrho.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbxmyxf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2efdogznm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2piiapbvr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cwmqcmqv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nmsiuvsd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2niinncri.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2azmwkoax.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dojajqrr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zdqrluxo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hkzxcued.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nizrfphz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tzgcksgn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lbjwggsy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2taenhrog.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jtfzrnxy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dooxcipo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2aagyubto.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wbszuhzy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ozctlhji.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2oxahsgoo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ygjjdcoc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2updzpyau.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qriqavpo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nrzkkiwg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fkiexalv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wuupzoru.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ttjdipyn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ewzfbvcf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bhvdhgub.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wsfrbvgm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hounybku.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lcvwydrd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ovzkiaog.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ptozmxva.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hghgzlsg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xkpoztay.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hfenwqwt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2srxxkipt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2atylului.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pyyawpxu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cdihxxym.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gkdkneli.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ldmmopns.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rowqxjjr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cybyuhkt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mudhxdmx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2pstuopuu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gnvgaaun.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2oevoezos.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2irhbarjk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2plnrmshv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qyyndwes.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qkqogfyq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmbsxbmw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fcwnrkal.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ctepmbdo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nwpzlwqk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ryeiexqv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pzammynh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pkncfpdd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jwwvnwmq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2igcizupr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2helgqmtx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2aifyosej.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugvarhhx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lpbyhvrc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bdcwfera.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aecudhtc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vqhjxdwz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwjryihp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ixhiluqy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2moiupnqz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2smbraxuy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lgcjmdsz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2styzhafg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2obrpjqll.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hvhalkjq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dqelpjye.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ahepkfxl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2teswnpaf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2revvrpyp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ebwqtztp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynjhozic.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mtstawcv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2luafycda.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2trlnifju.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yddvzhps.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yzqgbrpz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ulroytul.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjhklqo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ppdmhuzu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2edleeqio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bsswhloy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhavurjf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uqbxarab.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2foiormxm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcwowbcy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xnhpvnbc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zpxlwpdb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmawwgmq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pqfxsucs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bnrfczkf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dympbuau.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2luqhhnaw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ixvrefzt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zqkumrwj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jfvtlcyu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hmmztrez.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wmvtlgiz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2oaaamymu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2idseflyb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qitswhpu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wmnhqxxr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nufwdrsr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uweuyscn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2idoxzkwv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uutalysa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ngamolzc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nhemitun.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sejdkoxw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ylbghpjm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jzftexxc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yeehcvrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maodzezn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ifvxnxik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjfczfze.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvouotnu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2begnwjhp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dtfwgmnv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pzauiqno.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fqdzirng.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ovkuaqcz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hfovevmg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ogkpfkmt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lvjlkwgj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lmxphxdx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rlmvdxgx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxtyerir.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zzqfyyrz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ewqodqzv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cnfsfpfw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bckvsgqe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfcaqidg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2syjtdmtk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rsuanpje.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tpwotcue.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mytxfpos.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2blvzgymw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fzlbbfce.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dkhdwova.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dkrzqyzf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vsybtysv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwsqhumb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gybmtrgt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vrgqighn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzncvrh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tkopqems.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sqhviotq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yezcavth.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2equralce.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dictezri.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bdaboouo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vyyooqdr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ogazkfpt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fgagrnse.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ofphhnav.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ocfjdyjb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvyazaz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vyodqzuh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nomnfzno.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ekprvgom.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hgsxpjrc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nblrcrvm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gtbliugg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ilyzjcem.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2svgkdltk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qjahtjuw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wzlgfttq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lktovtnn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kssfdqbf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2unhuzwng.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xtyianum.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bburklua.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfxjinr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wlbidjxr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kqouavnc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2awxcuykz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2imkyzhjz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2giryyqrb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sljbuzvk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tzpqbcjn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qvcgmoad.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jcjkulnw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ryoqqwdm.html


<!-- 参考信息 -->