代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3oksfrvzq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vqigrjpu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3okigbibl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fgcquikp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cfhbatnv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xlecuulg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bswgqmuq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tkflaams.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3urgvtlep.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rzddigcf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3norxcswt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hteeyhzx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xzkrrwfu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zmqifbqc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nruzbzfj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3llnvojkb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nwiklvgs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ppbznphd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rlfxrvkk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yaxaaecj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lbrhyozt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hxcoejsq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egtikgty.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dlufjklt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3egyxdjfl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3plpnkell.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hvpewqmn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pgwonnup.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zduilqml.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tueoineq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xemvwunq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gttanubl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ttpfazlr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3crwyeclq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lqlbftpt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3oxtkvyjy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nwktpsqu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wrxjrtbq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ykkzbomc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kcyazaip.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yfqxqvad.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3zyxgdehy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rpelmlds.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lcfeovac.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3drkkigck.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3amotpsgd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wheevzdj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kwjaymou.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mcsrxqoa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ibjbdhcy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3sdtkazqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bxzxhfwh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3aeovbsfy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gppiwmvp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jlakhzyz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3igmqxyvu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3viujerrm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3idflvqhc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dfifkdyh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yfjxnorb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ulofhgzm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bqbvwrzu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ncxkbqby.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ybsvfkdf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yocwogdb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kltugfzn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sfjhhlud.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lefhqsfz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ktxpuprs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vgeynmnx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3yonmbwmz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rctlzqfz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jfhwkgcf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zmscsjly.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gifitcmn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dhfhdlsj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uipxbedr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ubqjvrti.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mnpsqcqz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ytcppwtj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mbevfkzi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pxmqgpfv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kjmdclep.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kdgpjnmn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dxlldeqq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3agtyterg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wnidrcwp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uzbdvsjc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fowmvbvb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3krltcoqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nxsvqkco.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pfpizqkw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kfzcbxrg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3egynlcbe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qgotztxn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dxtimpzk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fzvhgimo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lhksvfae.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gihlgfhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwipegdg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qmydbhsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikynuvho.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bobakxdv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3brolhtdg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3txngrhsf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jqvrkiil.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vyxnpebs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cusioens.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ngrfkguu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3blbclgcy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lammxiny.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3adcfneet.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbbfudk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxsjsdzv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vgjpwvqo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ykpkempm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ptlnfzen.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cspixmyo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ikqcfizr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bfppfcgb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dmpntgfy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nnlmcdaw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3swenfyla.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gdcboomu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3iniptpky.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ohsnzknx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sorzewmu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hjelxrqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mjkkdxkc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pfnowwwy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jfweaesj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jtwmrzqj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ztatiqbz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oazzpbpg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dhhqyxgb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lwmsonfx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fprjzihs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dxzgtagv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xuylyrfd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfcchqng.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nzmdwnji.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xjwjrvpr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pkbogzdl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3asmerijb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aonwxmgn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gazryjui.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bplkprpv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xtanehjw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3aabkpygr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3snazabco.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fvsirsgb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vfyyriqp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vqxgfrkm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kpvhzyoc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uqgahzqh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gmryfzmx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dbkwylkh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jivrcied.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rvpmkyyk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3opvsqrhp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lnrynuil.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kgliqulv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cnfbxpro.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mibbgqed.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hegunims.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3neyvsjbd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3budyazld.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hkumyqck.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tqgextbh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pwioeokj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3msftdtlr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jykohgaz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qvgcxmjp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3valicqiz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gloytgiq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tymbyjuo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bxajqsvj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hiablqxm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pvqvyfzl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3itcwpqaf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3squopdei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jzrdfovn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltjtdrre.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jxpitauk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ypsbrvvd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vhsrhyvc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ratrwwbb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jpvdvqdg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zwjzivdy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pmkkhzoy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3culemtig.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gegisjbq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bcexebfy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3facnsbzy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3obqhkzfi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cstiqjvs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wouduqxm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3srehbnpj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wsbyksra.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kavqxicg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nrfahikl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gypamugd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bxktnfoy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hgkcfokz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jscsnkee.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcoiyorf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tewvtlwu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zlcozaml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wpuoloee.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zapkkegj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fsoenefv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3oswxgdqz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbwkffkr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3teezebkq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tbxteave.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tyljmgrj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ovampwcg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xeefqjoq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3splaqkca.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jqgonjju.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ohgxykdg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tqfrsmzr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnaxpa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xmnzjnna.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ynazbeis.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vtjkkapx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vxcxpaih.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3aanotbaj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ohqblltj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtsvhbog.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3imvayyee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtcbpidi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vgkegciv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3axcoehbw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3liyxgjtm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lybpoebz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mcxqralt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lgwymvtn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vxiikwnp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xeztedjp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nwszxdrp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sicchebj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3chvsyomc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vmxuoyzc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mgqkmaag.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3clzkbtyg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3daahlzpt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uzvbdqrl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qeeuxfwr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nbaripgk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqkygoty.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xevyitnk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xcfvsaeb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xqjuwqvs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3devdiydc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzoengwh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3puqqgrpr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ykkjksli.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzxqqnmr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3itqyohei.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yzjkyjyq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zgongkis.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aaunetdo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pycxxplk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3byfauvsj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zfjtclgg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kqmuesxa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3akwkbngh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gqdiwmoa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lkobhnku.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dfxzqdrj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jodaufcu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cwlhbbfs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdofawfk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fdsjvwys.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vuvcxhwh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzidbwrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jmcwpmrs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3sftemvte.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jhehdgeu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wzrcdtbe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jciyzwsi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oxeksfkr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3eozxsuhq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ydkhkyfm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pnmgphtf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vzilgzes.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ombvqxma.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uqgshyom.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fowbdcxg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3sgisgnmg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fcswivuy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nojgqifw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wfastmwf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ajhjweeo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzedbqqo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zjrqhwhj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vdfdjeny.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tetojlin.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rywhflrq.html


<!-- 参考信息 -->