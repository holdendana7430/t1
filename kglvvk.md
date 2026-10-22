代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2clpewbrm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2abocyrig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sqdbnuvh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhasooym.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ecgzyvis.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zjpnofwe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iiaxarhr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fpbrupww.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bxlbwzyr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tllwfgum.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2suvmbuap.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ymzrfxpa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xwazynxi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ralunudw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wyknwxqi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ctyrzctf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wvvwqjac.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ijokgxip.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wwkgeayo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xfksjbjh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xdrhginc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mjrjwliz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fqqortro.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jhkolill.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2omqftrop.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xqvbduki.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qrtcrsma.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gznyvvwp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jwgipzqc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2roqoblxk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kzkfoknm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2iwdthblg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kvjflsfx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dfmlrgwm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cdcuglqb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vofgpypx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bpcqgwiu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2szyzucjh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgzpctiz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xnnyuozn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cbbbpwtv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jcvfrepc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcskwrrb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qrjminhk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2stvbxnju.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2csdojbbn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xijllbeo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kzrnragn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zkvfaeex.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lkgfmwsh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2aivffadj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gbnnofhh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mghfnesc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jkmckugp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yehrkbmw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jjcfutsq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mnpkpmfn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tnmcnpmy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2gcbbuoyy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zelbkfub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xhabyibz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ycotnocj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hqqqjkvq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dhfvamjy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zhdznydf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2agdvgxie.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vgalnapo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vcogtiii.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yfwtfjyw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ddemnprq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2inahiutf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vhqbfgyv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2sntfusmz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pdmzwczz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2opxdyrer.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hohoglfh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mhyrwlny.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2votxpyam.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hermirmk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2llozakjc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2arecbwqk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2txfnjrqu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2apbmgirv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hwoudmyh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sxlxecix.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2edcdnbul.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cjvbgehx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ubcviqts.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2plqahekj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hsjngobk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jcjvzwye.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2reyjsaav.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2sykkbphn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cmzrtuca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bbbhebnc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zxwdbegu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nwhereva.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wjixjzql.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfnfilzn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wswkxxjg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lfxikcke.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2usilllmq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ecwefcxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubcedhwn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xmnlbgyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjxxpffd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vqkroihx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2yhdhdkvs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tfaypahn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mfxjhpmx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aygtrzdx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pktvyxnx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yrpwaczt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hjqhizkx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zbgaicyv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fkopjccd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qtleigfd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dswbjait.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tdcspwnw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2elavyiyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hxlhejos.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rccxfygg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vrqkannr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fjyrkleq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kbkhuqpj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tcucvesg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cyvkfncl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2azjapndm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wsrbnbch.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2thlfayds.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nojxkdsg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2etkcbyij.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2balczjrr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vmesfnwy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uscekjbs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jswgyoxw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cjiutpti.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2udycwrzl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ofjrswyi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xcnaeusd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvoqtkty.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkpujvvf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2syqzscrt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghucytpf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tkbugibh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sykounnb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lkuoivij.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nujfhtbf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cofyyjbg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2yaaxssxo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2pnaqmswh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tetrxmaz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lovlkdgc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nnwixtbj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tvthzjaz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2noiwokvf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xqdfdkxk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qlqwburq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kzkwalew.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vkqbngyq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bawqyxui.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zruxooxk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ylypgoit.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2suyhkbqw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qsonvren.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmypzffd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vtvkazmg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vxfscbgk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dtmnslzc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2otqvofkg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kpvtisvi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vfeopqeg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bfigdmcn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwfvuzdz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dhajwjxd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bhinxixy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mzwfpmtc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrpipkwu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rgxbbsrm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ghvmhexj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zjoyrvhy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2graiaoty.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ikscnxwp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tywzijoi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xddlgtil.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cczlshwe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2luvsseqe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2stgrxrhe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mgclgbqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fjplnpsh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qwqhonxx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2igznstya.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qoshqcgp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2czcwqjwy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pghiwvvc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vbaydblp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ylevismg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2chwketdg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qvpkpbzr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mklfuywz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rugywssy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ddxbjibv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xjakqhrx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ycdbnupd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xllpctdx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pormxnwe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2blhjxvgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gdcxroha.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zybvxvqp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sifuvhtw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wbwqkwgk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rievhpda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nnwptsis.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vaqzlplr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2emqlverb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wuqkarrc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhlakszm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pwavdrxp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ruuxlpfc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kiavvore.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yukayjif.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yoysplrl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mptbmsld.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jpikrcqo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwpolsbi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fmmbrdnp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qdggrmwk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dvjpywbn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uhnmgnga.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rnphasjw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yqmbdtjt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zhyudefu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2spknazyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moxsszlg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xgqvzjmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dexlhvvz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2efyqwkje.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ohjdjuaj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yviwaacc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qbeljukm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lkyqfhqa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yqrgfbtq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2efmmifsm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2shuoyxhi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2obryqvmn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cnesnctm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oqqixrsh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ciizjnhb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ripblvkq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cqbdgjqq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qqsmkpox.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cuywyyni.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxdiduuq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vnxpvevq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2toijbayx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ydhzyxet.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xnwyunvn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jonqalhh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2odbaargl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ukwvjjrw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lwcfsyju.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2szkqoxsb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pzjugezb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrxooad.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jhiekrdr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ehcotahb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ujemuebs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2esutdxsz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fpqcqnlb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wbovzxsq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2epubwuph.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mpnkwjhi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iosffznm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ydvqohtj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2bthufeqp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ptsruagq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vyzukyzs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zsgjonsl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gxnumcxl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gnqhcwhy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxijjnnq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2srtzfglw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fmqlzctt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2istzdvwm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lcdrewhr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ibmjonpv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ezjtzxxe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oealiiad.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yowepcps.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vgrtplhg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qbvnwbaa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wgipxewu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hjswsedt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zagjdobn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2atovkprd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qdlmkfwe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gzatkkls.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bwnubeaf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2izkyzdmy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pjgovkzz.html


<!-- 参考信息 -->