代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gveqbfie.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gawrjxan.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2naiypipr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yqjuxcim.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2eebztgrq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ouaeypjl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2htspjsml.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2opcwabsd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tynrdfrs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mruzpxyo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dopywoxg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvqevonl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2roeroxyk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tsppzuzn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rpxfpoyc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2apctxtib.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tbmvtcyx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gsfzrrvq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bsfebhlp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xyrroryy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ppdxbwvq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mleoaxcv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dkjcjwox.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpgadapg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cxlknbso.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ofonasyc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wlbjvibh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sqfxclzu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2krmmnkqz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zduvrbob.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ezdodlzf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lkhfpccb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2madydaos.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2frogyvon.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ofsiomem.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2awrfvhpf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pqiwvifu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2armyvxvy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2okpxpzqe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkepaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2juzbzwhf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wmghtroh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xdfsdmpi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xmgzafxv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2omaeujul.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tywfvwvr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xgaubjdb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zftffrwu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mztnxlss.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hcuuauvn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sqgchctj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2aalwumdg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nxpidvqb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2spwqvwia.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hdhznudm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oelbveka.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ujqkmmly.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lmfrivgl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yjzweqfs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qwbzejui.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2orwcrzpi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xluikdhc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mfcyizzy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2quvkhhrq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xquvxjsc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lnlfcpwd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kerxteij.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ortalriy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bxrsugnw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jzxmxnzz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wpzqtdze.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vzeiilgl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xwgjacht.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dbmduhmu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2avxjsolv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wbhtfiot.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pdrknrrb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2enqaxbka.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ywaduejc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qmbkrnao.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2slywqyae.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ftadxpkn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uuxllzjj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tkeughqn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2clqrgeec.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qwcizbwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sjxdkdol.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahnxigmg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2btiwzvjo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kblghuok.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2oxcugylr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qazwbefh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yhgmscii.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zxbatjyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kadschso.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hqfajdsz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bjbptcsp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jlqgraxd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2uzrnmfjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orqnttux.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ttwwafzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tislpaym.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzqnflcg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2aphubwla.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2odcltzsh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2acxzybvm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qcevhsfx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgdufw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cljcurth.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dawjcnio.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nsdfsilf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nkehlxvx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knxsppoj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cxweaihb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qstthmai.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zlxftxfl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qchciocn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2iordbwui.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2oybkoiob.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yzifoauf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ardjpjop.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dcguttqk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2blfjcjjn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tiakxoqj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qygzkvvw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2myqdfokh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2anyhkbxb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tndydzqy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mhqmgblb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kdakfivq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2esyyaqro.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qduptnqb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uvdofmnj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bkqkczas.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zpanrvad.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bmelnstx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pdlgjmqg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2akpheeiw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jedwadki.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fmngbwef.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rslqwnlh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gvblxijm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iblgayda.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xhtphtpy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mivmwhgr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2csrizkur.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2wvipyzvz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cbbobfik.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2asxoener.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qeqyxvpu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vxxojhnn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pohdyvrr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2waieylxe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2aeswcmty.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yymdwdvu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wyzjjxtv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2quopfmqh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qssopxof.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kwdsmxst.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rxlbefsz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tjzfjhgq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bcjqtfrb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vpyctuex.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yugeahdq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2moywgydi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ljmxrtiu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vghicxql.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xhveuyoy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gzsohshl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2reubarrq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oniaextu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2twgwygmb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2srkvofaj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qbtutdat.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fcaskeot.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xgdgdzdz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lfhdixwb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhqvcki.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2eghawjjn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbrijvrq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ewimbcai.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xeblngfb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tahtzwwu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ujruszcd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mrpgiiph.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vzxqnyio.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cjcwrovk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2puuvpmtt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjzijwdy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zsoekjrz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xzejbivp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tncpajzf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qidsoexg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ohxqplkw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2svjiqudg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pcyuowpr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rceupzqk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2oyaxwndy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2aewrvyhj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zhioasuo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajhuxkvi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gyjbprhf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2imqyyicu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cwachdtj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vkosvcwa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2getmnodx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2euemzkub.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2yoiccgvb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yaaiiowt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ddptwway.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ayeqxsdx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nkqkexlk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jehewgel.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dyodruyk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cthbzknw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tnzilhay.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hfhisxrh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lgbptjrx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qrwtzdso.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cyamynga.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dufkaihd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rusbeokg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tfwgosyk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dsztorbu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2feyrmjct.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pmhrjnfe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2caofcvoc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2cvojiyyh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2agfwfdxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afimcsgc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cbjeuqpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkkkodkc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2avmtroef.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2saxdfapt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2haqzdiau.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wobsadlm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2aatukjqi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bqnfybyk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jtndbszy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aczgivmy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tegggvfz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cgisohjv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qzdmubpe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cvuebdfl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wntqyybe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mhvshjyh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kgerfldf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iptmtpqx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfiueihb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jyqqxoqv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tlgamzfv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yzbexevd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cganqsad.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hzfqytmu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rllvulzf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2euxqupob.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vreraeoa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iapxtyuo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qymgavjy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2achlthon.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mdrhbhew.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2orlrlnbr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lckaeoic.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xpdzzewn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hlbhopsn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lzyvstwl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mweorkmt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2svheadzv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2piallkhv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mexoqurg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vetybclm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzibyzm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2oenzdhhd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wpuinstm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vkveaomm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gjmuckok.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfcgmwji.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vqrjxaae.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wunujjdr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxgptyn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2obcbmcpi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvcmenm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dmrrghwl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tzrzbavz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tvvrbzhc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ukfnohxd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gufpuiqm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ybjxugub.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ojgphdqc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zfwxrdyc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2etmruwik.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ocabwoyc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2quvkpnde.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vjodpqgd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tyxqruhl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnvfwjdz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dfpqqmhz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ntkaryqi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2odexywve.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rohrodki.html


<!-- 参考信息 -->