代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.snrcjt.cn/gtcqwyzqpl.html

[R26] 命令替换
来源：http://hz.ydjk.org.cn/gtisvkkexy.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtkteuioas.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtleylauwx.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtmwzzxzco.html

[R28] 浮点运算
来源：http://hz.daria6918.cn/gtqnojwfav.html

echo "scale=2; 10/3" | bc
来源：http://hz.fengsongda.top/gtjbbtabhz.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtvkoktbra.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.andypj.xyz/gthpfbbjfh.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtxxiwtfov.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ppjwa.cn/gtrkbpsqbh.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gtcwyreupw.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtjsshrjyf.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtymwyadff.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtnpyxcldd.html

[R33] 捕获错误并提示行号
来源：http://hz.zhixingplan.top/gtpbyzmzuy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xylfe.cn/gthluymwfe.html

[R34] 退出时清理
来源：http://hz.dianchejie.cn/gtgccwbuml.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtbquplxyp.html

[R35] 后台执行并等待
来源：http://hz.pycfn.com/gttfpfseiq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtwraznipx.html

[R36] 并发执行多个任务
来源：http://hz.chenjidiqi.icu/gtsndeyhmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gtlnsbegze.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtefcaxflp.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtcnedkruk.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtszgcbfei.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zycfv.cn/gtqwnkywdo.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigfzy.top/gtknwnflxa.html

cmd > out.log 2>&1
来源：http://hz.ywan-chungtsiang.top/gtddkislov.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtpcrdyvmv.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtbtarvrrr.html

[R41] 丢弃输出
来源：http://hz.zycfv.cn/gtiycmchuw.html

cmd >/dev/null 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtokjeyqaq.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gtrqvyujeg.html

wc -l < a.txt
来源：http://hz.hammf.cn/gtacgtikqp.html

[R43] 按名字查找文件
来源：http://hz.sufxvd.cn/gtygbyxdrb.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtikuqywbk.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtuwvbmlcg.html

find . -mtime -7 -type f
来源：http://hz.cheryme.top/gtjpyjvsls.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtbtxdcssf.html

find . -name "*.tmp" -delete
来源：http://hz.tianlin.xyz/gtzwuojozo.html

[R46] 递归替换文件内容
来源：http://hz.yangfankeji.com/gtmjlvbtnp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtqcsqluts.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtzehaldfd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gtyayftckn.html

[R48] awk 取指定列
来源：http://hz.shzxlz.cn/gtbuxjgqeh.html

awk '{print $1, $3}' a.txt
来源：http://hz.jiagoushi.top/gtmafrrdlw.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtkgebzzvl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtymbovznr.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtavfxhgsr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtcqjkvuql.html

[R51] 排序去重取前几
来源：http://hz.dianchejie.cn/gtpwdtxjgq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pycfn.com/gtyrxhgdkd.html

[R52] 统计行数
来源：http://hz.yvedp.cn/gtowydiaej.html

wc -l a.txt
来源：http://hz.nanxuanxn.top/gthwsibrlx.html

[R53] 查看文件头与实时尾
来源：http://hz.hongshengwenyu.top/gtnyzkmmal.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.snrcjt.cn/gtfrxhkood.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtrfxfdgdp.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gttxdcxomc.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtskcaidvk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtnhebpfau.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtifdxtbwz.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtlivdfgld.html

[R57] 远程执行命令
来源：http://hz.vqdsnc.cn/gtlfmzzoku.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtqsnjxcew.html

[R58] 下载文件
来源：http://hz.andypj.xyz/gtotvwyvxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yvedp.cn/gtbqmugjua.html

[R59] 发 POST JSON
来源：http://hz.c1oappe.top/gtflrpxyyb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sweek.top/gtzrcxtjjy.html

[R60] 只看 HTTP 状态码
来源：http://hz.fzhhl.top/gtpkvwkzlo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtgiuvcoim.html

[R61] 磁盘占用
来源：http://hz.feifeiyinyue.top/gtqaxhvedt.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtpiduzgzn.html

[R62] 找最占空间的文件
来源：http://hz.dianchejie.cn/gtaaljwynf.html

du -ah . | sort -rh | head -10
来源：http://hz.cucudq.cn/gtujwuigtk.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtbvineqsh.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gtfaqokgkd.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtzmnarkma.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtwyzktzjs.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtcfpuaonv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtfsplqelc.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtyzuvzwxq.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtupxqohyw.html

[R67] 生成随机十六进制串
来源：http://hz.zhixingplan.top/gtgcgfmomy.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtccdxmpfy.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtvuppalxq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtklszqsrg.html

[R69] 生成随机密码
来源：http://hz.dashuyun.cn/gtmeotwcnp.html

head -c 16 /dev/urandom | base64
来源：http://hz.dianchejie.cn/gtnujqfkiq.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtufjsygai.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtuwelsvfq.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtgvbuqymq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtdymidrws.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtnnfugwvs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.haohaochexian.top/gtevmnqiir.html

[R73] 分割大日志
来源：http://hz.yvedp.cn/gtnvuxcxqh.html

split -l 1000 big.log part_
来源：http://hz.sweek.top/gtpvkergnk.html

[R74] 批量重命名
来源：http://hz.daria6918.cn/gtuofaibnc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cucudq.cn/gtcglblfiy.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtcahlnecq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtzgyyfyxa.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtneehztdj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtlnvdcwfu.html

[R77] 读取用户输入
来源：http://hz.sufxvd.cn/gtfjhiousg.html

read -rp "请输入: " ans
来源：http://hz.gaohongyu789.top/gtezxkajno.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangtech.top/gtmohvdtrn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tian-w.cn/gtjqbbmiqd.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gtrlyewkig.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cdnleiting.top/gteobyufaj.html

[R80] 查看脚本执行耗时
来源：http://hz.pengpengdd.cyou/gtxokokbak.html

time ./run.sh
来源：http://hz.iojbl.cn/gtnqeztnhv.html

================================================================================
来源：http://hz.hywenlv.cn/gtkkxnncnn.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtepilfnlu.html

================================================================================
来源：http://hz.fzhhl.top/gtfsjfoadq.html

[S01] C：Hello World
来源：http://hz.zycfv.cn/gtpvggvxbk.html

#include <stdio.h>
来源：http://hz.guowangkeji.top/gtxbojpydp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gttpemhxpe.html

[S02] C：变量与格式化输出
来源：http://hz.yvedp.cn/gthbbdndqt.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gtfzyqmnri.html

[S03] C：读入整数
来源：http://hz.smart0.xyz/gtiqrrfqzp.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtcnobagrk.html

[S04] C：字符串复制
来源：http://hz.mhx1999.top/gtaatvywzf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtlogtjmkw.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtlirkurui.html

strlen(s)
来源：http://hz.yueranfly.top/gtrubyjyze.html

[S06] C：字符串比较
来源：http://hz.0kj1m.cn/gtknduskus.html

strcmp(a, b) == 0
来源：http://hz.zhengqikj.top/gtbrzpzpuu.html

[S07] C：数组遍历求和
来源：http://hz.yonumen.top/gtloyzunht.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtcymlvxhy.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgufenzy.top/gticjgmbbu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtnaiemkhq.html

[S09] C：结构体定义与初始化
来源：http://hz.guowangkeji.top/gtfjgtxczd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gtjpttkeqx.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtqqowkhkw.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtziixcbyo.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtqymkrsdf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtiznaxiko.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tian-w.cn/gtjyuwwlqt.html

fclose(f);
来源：http://hz.svipenyu.cn/gtwtgutwvm.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtfvncsyzv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gotoacloud.top/gtfjbxllhq.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtdsevpoeg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yongpay.top/gtqqhkaoio.html

[S14] C：枚举
来源：http://hz.gaohongyu789.top/gtpxnlwdqw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgufenzy.top/gtcqahyvru.html

[S15] C：类型转换
来源：http://hz.hammf.cn/gtexggindz.html

(double) a / b
来源：http://hz.tian-w.cn/gthlafwfrp.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtxjmnrgmb.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtgructfrc.html

[S17] C：安全拼接字符串
来源：http://hz.yuanzhike.top/gtupgbgvuy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtkqvuxvgn.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtawyonyca.html

int main(int argc, char **argv)
来源：http://hz.cdnleiting.top/gtonkfxqcy.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtpmcmgxtv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtmknkcacf.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtlbjqlrom.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sysykeji.top/gtgoxrgmrl.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtlcgendee.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtomapgyiv.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gtiaghhogl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zdqjudy.top/gtozssjtsl.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gteblmjuqk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.52xcode.cn/gtgpzisfwz.html

[S24] C：获取本地时间
来源：http://hz.9152youxi.cn/gtblibbbpj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gtrhyqdqgx.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtcsbjgelb.html

memcpy(dst, src, n);
来源：http://hz.shuidangran.top/gtjqivbawp.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtyebfagly.html

memset(a, 0, sizeof a);
来源：http://hz.xylfe.cn/gtrukdoxim.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gtfocohtwh.html

const double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtdeqhtmnj.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtljmokees.html

static int counter = 0;
来源：http://hz.haohaochexian.top/gtdrdzxfvs.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtmebtrzcj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtrfqkyrea.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gttuffcoxz.html

#ifndef X_H
来源：http://hz.quarkkingdee.top/gtlpjvkszg.html

#define X_H
来源：http://hz.nanxinkj.top/gtaodygguz.html

#endif
来源：http://hz.ivvv.top/gttjcjtxdi.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtoulzwhge.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtdaayhxhg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhixingplan.top/gtokrrtpur.html

[S32] C++：字符串
来源：http://hz.haohaochexian.top/gtpffiriye.html

std::string s = "hi";  s += "!";
来源：http://hz.dashuyun.cn/gtsexioymk.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtvgxuigjd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtzjcusyum.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtiddqzpiy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.bjfxy.top/gtgmldhzge.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gttgfnrcbp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtvikuhrsl.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtsjfhoquo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtnxpvyxpg.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gtjkvyywff.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtndvcopcn.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtglghbqnh.html

std::sort(v.begin(), v.end());
来源：http://hz.ydzc1.top/gtqcvxieqn.html

[S39] C++：自定义比较器排序
来源：http://hz.hfpthk.cn/gtcsoxlzra.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtglbggofo.html

[S40] C++：查找元素
来源：http://hz.gogol.net.cn/gtzlqhyqup.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtymcqhwwy.html

[S41] C++：类与构造函数
来源：http://hz.yj20258.top/gtniykzqec.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigufen.top/gtsndlvnvh.html

[S42] C++：继承与虚函数
来源：http://hz.birdmap.top/gtemfmrzls.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhijiandao.cn/gtbtisajyu.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtsjltuwlx.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhijiandao.cn/gtozzuvykt.html

[S44] C++：引用传参
来源：http://hz.fzhhl.top/gtdsuumrtk.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtffmojftm.html

[S45] C++：lambda
来源：http://hz.chenzaomai.com/gtpbsfacwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtilbnxlmy.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtakiqexwv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gtieoyrfcl.html

[S47] C++：结构化绑定遍历
来源：http://hz.c1oappe.top/gtvmstnydj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtpzwjiimd.html

[S48] C++：逐行读文件
来源：http://hz.zycfv.cn/gtbcvgeqsw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pycfn.com/gthnylryzu.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gtxduvsuss.html

[S49] C++：写文件
来源：http://hz.shanyushiyangtech.top/gtgxzsybgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xylfe.cn/gtueojzksy.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtcqqljbet.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtfrldklzx.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtwaxnfasu.html

static_cast<double>(a) / b
来源：http://hz.hfpthk.cn/gttefcwbtq.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gthriqakrk.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtxqndsang.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtotfmnmum.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgfzy.top/gtyrazczup.html

[S54] C++：异常处理
来源：http://hz.nwbrower.top/gtxpcnhspg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gtigrctqks.html

[S55] C++：结构化绑定
来源：http://hz.xziqi.cn/gtttojnuuc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gtcqiawyla.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtxefwejdz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtgykgjqmu.html

[S57] C++：编译期常量
来源：http://hz.xinyue.icu/gtxojnwplz.html

constexpr int N = 10;
来源：http://hz.yvedp.cn/gtsxxtnirx.html

[S58] C++：命名空间
来源：http://hz.hongshengwenyu.top/gthadvopgg.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgfzy.top/gtgedzfuts.html

[S59] C++：静态断言
来源：http://hz.kuanghao11.cn/gtewkcqrhr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtmyigcjnx.html

[S60] C++：遍历并删除元素
来源：http://hz.0kj1m.cn/gtkiltidlo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtkalyzqgt.html

================================================================================
来源：http://hz.yj202588.top/gtovbyohdm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtxgbdgsch.html

================================================================================
来源：http://hz.c1oappe.top/gtdidtvlfs.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtznaniffx.html

println("Hello")
来源：http://hz.smart0.xyz/gteatjqkyw.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtbglplexe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtcxpiojuv.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtlapurrxn.html

"值: $b"
来源：http://hz.meibo888.top/gtkesudxse.html

[T04] Kotlin：空安全
来源：http://hz.zdqjudy.top/gtqnapevbw.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtbtzkjwnt.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtuwuqrqsd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hammf.cn/gtcjrzciur.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtcwoxgakl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigfzy.top/gtbqzuckat.html

[T07] Kotlin：集合过滤
来源：http://hz.xinyue.icu/gtogpzziab.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydzc1.top/gtzmynzwis.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gtgwwyvtkk.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtemtxrjii.html

[T09] Kotlin：扩展函数
来源：http://hz.ybcxt.top/gtssdkmczf.html

fun String.exclaim() = this + "!"
来源：http://hz.hongshengwenyu.top/gtjmqzjgol.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtvvmjbioq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258888.top/gtxwendweb.html

[T11] Kotlin：协程
来源：http://hz.vqdsnc.cn/gtacpuogos.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuanzx.com/gtjemyqgne.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtysbgpylt.html

val (a, b) = Pair(1, 2)
来源：http://hz.dianchejie.cn/gtjvlncxzs.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gtgnekewnd.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gtuumpnnru.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtbrycpggn.html

for (i in 1..10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtcpmcxoso.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gtosezszof.html

interface Shape { fun area(): Double }
来源：http://hz.shangyingyoupin.top/gtgfanjweh.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gthuglwvtk.html

print("Hello")
来源：http://hz.zdqjudy.top/gtgjzrhksn.html

[T17] Swift：变量与常量
来源：http://hz.svipenyu.cn/gtijbklhvp.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gttlvposkr.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtzlnhasfw.html

"值: \(b)"
来源：http://hz.nanxuanxn.top/gtyetivqqg.html

[T19] Swift：可选绑定
来源：http://hz.hywenlv.cn/gtqslmystr.html

if let n = opt { print(n) }
来源：http://hz.zhijiandao.cn/gtvqcfsbix.html

[T20] Swift：数组操作
来源：http://hz.ybcxt.top/gtxrkwlvoc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtdyhbixjj.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtlulzhmdn.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtpclwzyiu.html

[T22] Swift：字典
来源：http://hz.xinyue.icu/gtswtscvfb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.mhx1999.top/gtpbwyvbdk.html

[T23] Swift：函数
来源：http://hz.quarkkingdee.top/gtzgonodze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtjrsbxaea.html

[T24] Swift：闭包
来源：http://hz.nwbrower.top/gthxkygedi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenjidiqi.icu/gtsmrvdmhv.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtjhybimhj.html

struct P { var x: Int }
来源：http://hz.zhijiandao.cn/gtdrwtyrkn.html

[T26] Swift：类与重写
来源：http://hz.xziqi.cn/gtvpzicjes.html

class A: Base { override func f() {} }
来源：http://hz.chenjidiqi.icu/gtkozhejue.html

[T27] Swift：错误处理
来源：http://hz.316326.xyz/gtvixeqsud.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtuiwubdln.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtyzetwena.html

enum Color { case red, green }
来源：http://hz.ydjk.org.cn/gtuegoefnq.html


<!-- 参考信息 -->