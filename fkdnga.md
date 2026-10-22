代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rvkdzwkr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qrhdxmim.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoqdagfk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zhdljbto.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qgthozvl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ofcrmcfh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2phhamhcb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mhhruzfn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2livdayhb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2scnruhzw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wfkojzuy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wbbqmgbd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xudaolkh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2otbdytnk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2eblwykwr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2foothwfc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qvdsteaj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fcpomdaw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hlbbupkg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fjznkhio.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zoctkozf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2amljqxhc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgsgkpax.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2chafzdje.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wofsrldq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nexjpdcw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hiclrwxm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fiqwfybn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2syfsfovp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vmxhfkja.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2osiyqpfw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zhzaeekl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2znzecqkk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2aepczsbo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2alggnjxd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fntqwzkm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vaeivcgt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2evgyxkwc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ltzluzeb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2urxbbzyj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2susawaqm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kmacbguj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eqbsrzgn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jzzuhrqy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ekqccgdb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxnlikbz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cyqlgtwn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2atzzipjw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fyxdaqun.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ygqvbdqb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2thlszvsa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yxzpozov.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rvyhwbtz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jspucymv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pcbmzkhi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jgyutnko.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hfnvdgtz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zzynbdel.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bfnlhotp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2djhaglfn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sayphcvh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pagdtgjm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jxwqmrmo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lmuzemcl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bxdkzoxx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ttqpjnqh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xyqmfdfs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2unvkpkxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fkqzsaec.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lyxlnlki.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2klkuydkp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2umdtvvwq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ueasmffy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mswnzaaw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nxofemwh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vlrnzugo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wnailayd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sqtdndji.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sjhmfhgx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2txmcrqtp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rsohucak.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wmxpwvhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uupenqyd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rwnjdjrp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qytdhwbr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2piwjppoo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdvyaeri.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghyywvqj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yeqiuvgt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdwifzyd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yffgwrbj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tmsgkvdq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xjgkxqqq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ewbcppan.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gbytvgsq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jwlmlelt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2axgvthbo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mqgmvpqt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cwmejdjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2woilwaih.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hyexavnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtsgrmsb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ciywqfdo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pkaryehu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2khktrwqf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ybgsdndk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xtkbnhxj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mtgcfxuk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dwgbptbf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nvsftsmu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2knogvlvk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cbqudppf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjmrhqz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2anirhhxz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2sslbokhb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2osnpbkhl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sxdrvnkb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jljkyrdk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zptxskki.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ffcgixpe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pmkkkmzp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qvftdkah.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dzrltdnd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qjlwsudw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pcchnoeo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hgfolhot.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2quenbbja.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zhtarfwc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ohibpavs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vvbimckp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ggcoljjm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2inocakvg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2pmwudhrr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mezaymbg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kprcrbws.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2omctkfsw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akcibxfj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pjjslsbl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zfiqwcsb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gncnulax.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzsonjs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2irqsogsc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sltziwhs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2klvisrje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ygkieink.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fzktribl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fewlepbj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lzelpokx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xhhdblia.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ouhptjsp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eibrewtl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jetbrrag.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cxiggqsx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2edsbvghg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vxduvdhv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2otnqfhsa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qlsbhnrj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ththyfbj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zkvgekkg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfcihpty.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qniqrtzr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rftilehq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tawryqnz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cevfwefs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ozejjzwm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cffjvqvj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nzswbktw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lsxhexgs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wptbjzki.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gnvxkpes.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bkfvhril.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2apxzirxq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bnqonvzk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vopkusxu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wjesotqi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mmgohqvs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ejpucjtb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rqfmaqxa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tvovhpfo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gauwxwfy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2npghzukx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nrmjmngd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vatgmiqw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ompmhbgh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mnczdaqv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ihiccbua.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2eatbewrb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aambzdzj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytlywfqf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kvvtzqsc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bexkxsiy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2acznwbzp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ftnrlvji.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rrcvsodt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jhligpwm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lsmxajxb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2whvwlztv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sqntgcoo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2utojbajr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lhflnosx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rjyopsie.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxhlolyv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtlzpzkr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qiypwzir.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kenzmgux.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2skdofhjn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2laisearf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mriypiis.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rugfmluv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ttmcgpgc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nmsvxuhc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dggwoosx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjbeeyo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gnoebdlk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mluytakw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2bvshaoho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ebagygbd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bjdecbys.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dtcyiwqu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sklpurzq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxnirbic.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vngulvjp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wipsqemm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rlfpaket.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2blhfsxch.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bmahkjut.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gknzbkot.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tspbxlbr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ffkuuwyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpuhpjpt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oysycwfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihddfqal.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hpgbkwrd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2carjnfbf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hfiuncfl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qkekrorp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2flphdipv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cwbbftot.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gqdumiqd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nbebxfii.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ycrybrpc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tacsfpbg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nnvsxcvd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kdswmwkk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mmnbafrg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pasmjhmk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2parfdlhq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zxdflyth.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlzidmdk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yvzasjtp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjkkvixl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wxewrkvn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cqlrpsfn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sfrinwca.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ngzmntyn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2icydlcsl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qzsiyvzw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcucnca.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojzucnca.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qeddppyg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rmlkpger.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tatmhvbw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdkcpsxk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nvitpypk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2aobwvqth.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gnozijwe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mrspsshn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ptyikttz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jpxifctb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ndctsoqa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jxkhczjq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uonijauv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wvrgdccc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nrhgcvla.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uuxhscqi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rsuwrtax.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvzbyqdz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fvijemlu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mrhuhtct.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxuswlh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vixdeuby.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dyyqjtbj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zcgdawdl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wekvyuhu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bgxxqdjm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2glkwydds.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lwmqyeyy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2caiqnvdg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rhmohhcx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2anhuhaxm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ivhjomsg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wkiizpnh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2laswvgou.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2moxdwqtp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2aoqhkbxi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2avwwbpjr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cjarojwo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ewbnwtmj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dwgdaqya.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jlcmiefx.html


<!-- 参考信息 -->