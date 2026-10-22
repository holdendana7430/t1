代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bslftdym.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jiktgekk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2psbfnxbw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kxjylyqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zhbvqoxs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2twckmfaz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gixmriwe.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2emruqooy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tprecanl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bmbatuvy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2awpiaqrg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2onzuisxc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xsqllxan.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pmmgmryb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jvnbbpln.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ouxvnlyi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zvpexqpp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kmoarefo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2plbyvwif.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sqzhdzvn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vvbervgt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ifwxucee.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kuwttqtg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2irrosyrl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nkgenwpy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ygnajsip.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yotqokkb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oometjyo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2emtaoysp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2igspkwkg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fxvgyetb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wgriwlqa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pwlvexga.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uptthhyp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2smkcuveg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sagggryk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dfvwhgsm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nmizosqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qjnbnhqe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2quayqugk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nqrsxnja.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2edajwpfp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qrzaghrr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vlsovzsa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xenzqbbx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfpswufy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykzucvyf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xhwisgfl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fowaykyu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vvipixad.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qkwixuja.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wwsbsask.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mxppajmy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvlvdplj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wsdhsejo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xegitprt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hbzzzuxf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmuwft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2uljmapem.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wqjjplil.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wuytzrcs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2afaybksg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vfthgkmt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ragdlwns.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rsqkfobb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2orzcyeir.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jmyuiomn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rwwmglnw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dhwbudgz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ddoeyccm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lftfpkan.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wvpskmja.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ifqcyzdg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mkmirevn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rtjwtovi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2krscpred.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jiwhpyys.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bfewmofm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2lqnfxjna.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qkmeteue.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mdnhqbix.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2adsrrmrl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uhwkpphc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lpafpsol.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dzcufedg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2iabsjpqj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2axdkeoxn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2pespfxqn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2huccvatw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2urtteegq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kcewbllz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wdkiouyz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2uczyfoaq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nfrqpyqt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ngyxzwbu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jinwwduk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fkgsxgrq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2edzzshph.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ozdwzble.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmmbijcp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xjkaimio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixanldrv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ijetzocz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bdvaawax.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2aceubnjs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rdmkctpz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2juzcinuq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eaoflqpn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uvngyapc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zlufpecl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cnakrfzb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bloijvsi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nvxijqgq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nxivmcfx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nssvtkej.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fzyqazhz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gmiyczqh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ymegleyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2klesnxwu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mbgyurkn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hahciutz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xstjktga.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qejsxjke.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xilyjerq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kdrotxfu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dsjvpnpf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2blhawotc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccuszaxh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vferdltv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2psiqditd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vgdxyoib.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qfqzkvme.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ztqjbbex.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2diwnygwo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kczfweiw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gznmwpzk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2phoisftt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cvvwazwg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dsjnqyec.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ytggsrqd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qeafqrhj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ptfbzpud.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tmxajogk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xvwtljbo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fajaktnq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gewcdgqu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dsbgpagv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jiictjnj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zrlovhmy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xpcuikkp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xgfhnqpt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tnuvtmvo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ghnllahi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nozjaiqf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mqrglost.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2whqbusca.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mdjkcvsx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ohamqaxv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ykloubdl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymgagfhs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2caxdwemt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ebamdnqe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yvzpuayl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2islcukdg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ridhvobp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2itrimndm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kybdnhtj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cneisyjc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mpzerghk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dhodkddu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uubmibcx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mwezppdn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lopindbq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tyejkqfr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tfeemmyq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzxxrtpv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jlwmbbhg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2inibqlzb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2psjtjdlc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dffxqekf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2euypuzjq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tcpjqddi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmocmxnx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2thvlhdku.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gezljegn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2eprketfh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rpraseea.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mraspszw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bzejdfmf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kwcomoum.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xtlocvtn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hdthtema.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2oknhhuqo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nlywvnhb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2nrvwxqjd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqwxxoai.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wfqzvpxh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2duzefonw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2skqyjoga.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bntcaswu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ajqlkwpu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2drbouhdd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cghrhjbv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2itmynwhg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2flklqzbd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hhoddwrm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2adwyrkqb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mibsbhvj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2srihacte.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2agtaiosk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gufkuqsu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jvwtbawl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zixdzgec.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vswtecbf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qhnyzcfo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xvcwgkgk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xwbqetmx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rcnwldpy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bygdxwyh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2amgrxime.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2naeeoyjz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wzeaclpr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nmguclmh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uqnalemw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvfzdom.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wnzeubfr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lizsojin.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xcjluolx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gkedkxkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2espmyomp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ukbelwuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnejaunm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jnvqsbjm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hejwcajd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezenrpzs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tjhytyxx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2emgyylhi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eaimmqxw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tkygfvav.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ukrxkmdv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qvwytfdb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yzfnfecl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lrcsdner.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ptdgagnu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kqjazbux.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kitftulz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fmzezqec.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rodnjlqv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kpsdykar.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2njnwcegq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cvjmsfds.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vfnwrcyj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tahfrcxz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lkxyvfij.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2btrrusuk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xegavkus.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jffgsdyo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2argvtlfm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kpjsdubi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qzcymszc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jyjlhxlp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ehwwxnvt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hupkbwpn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jdbutcxh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ajcjkhek.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgbsvwam.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yettskbf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2alfpfjpg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jdevrwpk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhoorcm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qmcidqli.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bmmaaakg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uhdhkkys.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vmvdyuvi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2unugyokn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2icnnenoi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfnkvqzq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uhssqeyf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nqfjeltw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfcgdrwq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kfzxpypk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wlsdymze.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tqjletbm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2znyxjnzn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ibmobsnt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2filgdzuv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2psazyjax.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lbhdhzms.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ayztgetx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ooikxnwp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wvfuilmp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xpjqlyct.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqsfxloi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ljmzmqty.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2njvxjaph.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2obknftiz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2znzrdvmw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2orvmchnl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2liuykifq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cuvhudos.html


<!-- 参考信息 -->