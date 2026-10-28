代发 wailian999

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtpcioxirf.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gtszrczrbp.html

echo "${s:0:5}"
来源：http://hz.hammf.cn/gtauktqjnc.html

[R23] 字符串替换
来源：http://hz.birdmap.top/gtnkfjsgkr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cucudq.cn/gtazmafycg.html

[R24] 大小写转换
来源：http://hz.gotoacloud.top/gtazzaxmma.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gtdmhniyly.html

[R25] 去后缀 / 去前缀
来源：http://hz.ehwqpu.com/gtngxvgfag.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtmwzwriom.html

[R26] 命令替换
来源：http://hz.mhx1999.top/gtggozweax.html

now=$(date +%F); echo "$now"
来源：http://hz.birdmap.top/gttolwuaot.html

[R27] 算术展开
来源：http://hz.9152youxi.cn/gtgfebxlwk.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtayxmpjtx.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gtzssgujlz.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtezhauzcq.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtadeviqxv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxinkj.top/gthdseuybb.html

[R30] 函数返回状态码
来源：http://hz.yj202588.top/gtkbfmuwnf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtrecgpleu.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtgwwcsyst.html

f() { local x=1; echo "$x"; }
来源：http://hz.andypj.xyz/gtqsrwuwqt.html

[R32] 参数个数校验
来源：http://hz.haohaochexian.top/gtkaxvtdtl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtagttiugr.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtgirjbrrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jianghu66.top/gtaazvjosw.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtehbrjjhp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gthqlsksuh.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gtxweeaeql.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tianlin.xyz/gtfvudqvhv.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtmopcgilg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtartglcvs.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtufvtyukt.html

files=$(ls -1)
来源：http://hz.zhiwuduotai.top/gtepiyquyu.html

[R38] 管道串联
来源：http://hz.shzxlz.cn/gtrltkixel.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtbadzcelh.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtleyjymyb.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtmuxoiqbl.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtbiouhxtg.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtwyxtlsqt.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtnmglqmwz.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtdszygtwg.html

[R42] 输入重定向
来源：http://hz.cucudq.cn/gtfjvzqudy.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtbqwchqhe.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtkkxfyszg.html

find . -name "*.log" -type f
来源：http://hz.cdnleiting.top/gtmdfrlsnu.html

[R44] 按修改时间查找
来源：http://hz.aizwys.cn/gthkvydull.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtfutogvah.html

[R45] 批量删除
来源：http://hz.ydzc1.top/gtlbpfjuuh.html

find . -name "*.tmp" -delete
来源：http://hz.cheryme.top/gtbkntnnuj.html

[R46] 递归替换文件内容
来源：http://hz.fengsongda.top/gtqcqbxsfo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtmeiibqii.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gtkpiblwqo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtjsssxghg.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtzfqlxtcb.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtelyrrqlu.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtkbakvfxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aibaodan.cn/gtjxzmcwrj.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtavcmyhnu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gotoacloud.top/gtyehemxfv.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gtcwisaate.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aibaodan.cn/gtcgngpifc.html

[R52] 统计行数
来源：http://hz.shuidangran.top/gtqqkslyoo.html

wc -l a.txt
来源：http://hz.jianghu66.top/gtwicydvwn.html

[R53] 查看文件头与实时尾
来源：http://hz.havefunace.top/gtytrrjfxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtzegyhfrl.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gtegwyclff.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtduewfprt.html

[R55] 压缩与解压
来源：http://hz.snrcjt.cn/gtcfnvfxtq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtlkgucsjj.html

[R56] 远程拷贝
来源：http://hz.ivvv.top/gtewwycimv.html

scp file user@host:/path/
来源：http://hz.hammf.cn/gtpiybllyk.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gtuppexpnz.html

ssh user@host 'uptime'
来源：http://hz.ivvv.top/gtjvznknqj.html

[R58] 下载文件
来源：http://hz.hywenlv.cn/gtkjbmwaak.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtejflysyz.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtwhjwzjxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zdqjudy.top/gtwrozwkdj.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtmnluvgmv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yangfankeji.com/gtkhytszpy.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtphzdomnq.html

df -h;  du -sh *
来源：http://hz.smart0.xyz/gtchjxwstg.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gtmipwlypt.html

du -ah . | sort -rh | head -10
来源：http://hz.shzxlz.cn/gtltiolkfa.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtaxvpmtlx.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtlysoqsrc.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gttkxmdzpv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gteoejqgzd.html

[R65] 查看端口占用
来源：http://hz.yonumen.top/gtvhvtqlcb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtfutiypbd.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtltzryhjv.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtkcnmdjix.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gtwvfvornx.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtdvawwdbd.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtvuballsc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtttkstibm.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gteajjtfef.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gtgnwynggy.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtgeikejop.html

date +%s;  date -d @1700000000
来源：http://hz.0kj1m.cn/gtzyaynjzo.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtasxekrbt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dashuyun.cn/gtlvgloobk.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangtech.top/gtvspyzzot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pycfn.com/gtmyugimsk.html

[R73] 分割大日志
来源：http://hz.hongshengwenyu.top/gtiabkzogn.html

split -l 1000 big.log part_
来源：http://hz.ivvv.top/gtbdhwpyvn.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtfgdpqtqk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gttdrwucpx.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtnrglssnr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtnwylvotf.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtmcdgotae.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtcagilumk.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtavgpdyzt.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtmrapsmde.html

[R78] 交互式菜单
来源：http://hz.0kj1m.cn/gtmejdrcza.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtmqhcouwf.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtpfkzylfg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pengpengdd.cyou/gttjuchthu.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gtrkjbzggm.html

time ./run.sh
来源：http://hz.kuanghao11.cn/gtbamqyawc.html

================================================================================
来源：http://hz.daria6918.cn/gtvjaizyod.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtpsizztlx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttqpxndrp.html

[S01] C：Hello World
来源：http://hz.yongpay.top/gtdkvpwjzk.html

#include <stdio.h>
来源：http://hz.gotoacloud.top/gtghbabkml.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtbgaprgbw.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtyfutuehx.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtmkvzujzm.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtjsinismz.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtrciszzbg.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtpgrfejaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tianlin.xyz/gtscblmwso.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtkjsfxqwq.html

strlen(s)
来源：http://hz.kuanghao11.cn/gtrgsgfsqa.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtlsrjmolm.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtnyaatatv.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtkescdaga.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtdjhroorv.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtfyiatslf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtaxqxwhio.html

[S09] C：结构体定义与初始化
来源：http://hz.ywan-chungtsiang.top/gtcpgwhhjz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtkwcykptk.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtmsnyhltu.html

int *p = &a;  *p = 5;
来源：http://hz.hammf.cn/gteupzuxcy.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtzvxlobil.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtshoebcgy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtciqznyxq.html

fclose(f);
来源：http://hz.jlsjyb.cn/gtkxpunquz.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtebsabsur.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.c1oappe.top/gtsncmdyav.html

[S13] C：宏定义
来源：http://hz.yonumen.top/gtgsygxvlk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yonumen.top/gtqnqudxwu.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtsrxyjtkl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tianlin.xyz/gtzptwhgjz.html

[S15] C：类型转换
来源：http://hz.zycfv.cn/gtyklrqtdf.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtftseidjb.html

[S16] C：位操作置位
来源：http://hz.snrcjt.cn/gtgqyzchzj.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtqmymyuzs.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtpobwjeyv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtitpsanxa.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gtfpjumlbt.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtlfvznixy.html

[S19] C：快速排序
来源：http://hz.tanke756.top/gtckakwdch.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtzoknvczk.html

[S20] C：二分查找
来源：http://hz.ywan-chungtsiang.top/gtigscrjsx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtjckxxyta.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangkeji.top/gthabhrndm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tianlin.xyz/gtaoolchqr.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtvbrknflh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cashguo.top/gtwwowhyge.html

[S23] C：随机数
来源：http://hz.52xcode.cn/gtnkohigms.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hongshengwenyu.top/gtarxabdyq.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtytzjybyx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhengqikj.top/gttttxsqeb.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtuilxhmvt.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtmturqhvg.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtsxlrvdqs.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtfarvbnkv.html

[S27] C：定义常量
来源：http://hz.shangyingyoupin.top/gtehqajael.html

const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtbrfkjacy.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtuuonfdvy.html

static int counter = 0;
来源：http://hz.daria6918.cn/gttqjzxhil.html

[S29] C：变参函数
来源：http://hz.xziqi.cn/gtjquctlkc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.havefunace.top/gtomztcysn.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gtmtnskamy.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtayiuqrox.html

#define X_H
来源：http://hz.jlsjyb.cn/gtolfyenuj.html

#endif
来源：http://hz.jiagoushi.top/gtsutfmzhs.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtqknpntbw.html

#include <iostream>
来源：http://hz.xziqi.cn/gtupjccprz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dianchejie.cn/gtoyjcekqz.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtksdazemj.html

std::string s = "hi";  s += "!";
来源：http://hz.tian-w.cn/gtcafooyjh.html

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gtuaskusil.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtxdluhdji.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtwoafquhu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhaomingkeji.xyz/gtotucmfjl.html

[S35] C++：map
来源：http://hz.zhengqikj.top/gttuxbluiu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtlgppdlju.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtwrmpxmen.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtgmrcegtf.html

[S37] C++：set
来源：http://hz.cqqwz.cn/gttojcigus.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtydqgdull.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gtctprodgk.html

std::sort(v.begin(), v.end());
来源：http://hz.jyoumei.cn/gtqbixtufm.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gtxyaqxsdc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ybcxt.top/gtvhcnsmki.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gtryjworbq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtgpxgcpso.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtwhesmidd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gtwlgzkqog.html

[S42] C++：继承与虚函数
来源：http://hz.chenlongwang.top/gtrdfowbge.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtjafkzpwa.html

[S43] C++：智能指针
来源：http://hz.aizwys.cn/gtlpilpgkv.html

auto p = std::make_unique<int>(5);
来源：http://hz.jyoumei.cn/gtynwuvrce.html

[S44] C++：引用传参
来源：http://hz.redwolf501.top/gtejrqmvwa.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtwfaouell.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gtidebjxya.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jlsjyb.cn/gtjkhzgnzo.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gtpmqnrcai.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtigrnzpbb.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhijiandao.cn/gtgecrpyjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtqpzygrwp.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtvvidzkxz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ivvv.top/gthlhyghwg.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gtimxbzald.html

[S49] C++：写文件
来源：http://hz.daxiang520.top/gtngmpkmet.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.smart0.xyz/gtdwjgtrcr.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtikvqxhce.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tianlin.xyz/gteaquvaix.html

[S51] C++：显式类型转换
来源：http://hz.iojbl.cn/gtehjlfsgp.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtemaskmxt.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtikmhfoki.html

int size() const noexcept { return n_; }
来源：http://hz.fzhhl.top/gtruhnoezv.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gttqwkwxgc.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtyqxtmpgj.html

[S54] C++：异常处理
来源：http://hz.nwbrower.top/gtbiqrwagy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtdnlnzwsh.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtuxkcbjsn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gtfmvtsqez.html

[S56] C++：optional
来源：http://hz.chenlongwang.top/gtlrfpnxwf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.iojbl.cn/gtqtbmrodl.html

[S57] C++：编译期常量
来源：http://hz.pycfn.com/gtporsqcas.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtdjltuuuu.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gtespowhml.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydzc1.top/gtdgubzauq.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gtoojviosu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtoyfmlxzb.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtvgwercri.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtusnjyuhr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgrhifmfo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtmukdxzmu.html

================================================================================
来源：http://hz.ivvv.top/gtpjloirte.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gtxtjfpuvw.html

println("Hello")
来源：http://hz.jinqigfzy.top/gthzfsnzul.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtgltorceo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.feifeiyinyue.top/gtzjmgmqqv.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangtech.top/gtptxevwvr.html

"值: $b"
来源：http://hz.ybcxt.top/gtkbsujkuq.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtwjdkayax.html

val n: String? = null;  n?.length
来源：http://hz.ehwqpu.com/gtlqmimzqs.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtnewjzgtq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sxryk.cn/gtvyqftvqa.html

[T06] Kotlin：集合映射
来源：http://hz.hnxiangtu.top/gtjygrmcxg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtpklhshlc.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtoxqyirww.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cqqwz.cn/gtjomfsodh.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gtzfxazcsl.html

data class User(val name: String, val age: Int)
来源：http://hz.sysykeji.top/gtncnqzckh.html

[T09] Kotlin：扩展函数
来源：http://hz.zhiwuduotai.top/gtcwfcbfup.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtmpsnavys.html

[T10] Kotlin：默认参数
来源：http://hz.guannengcc.top/gtetvuordg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gtpgivolmz.html

[T11] Kotlin：协程
来源：http://hz.yonumen.top/gtpljdmufj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gtsbomsvnj.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtrapllltb.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtdztlnlbp.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxinkj.top/gtgtqiqsiw.html

val m = mapOf("a" to 1)
来源：http://hz.zhixingplan.top/gtmyqaufcm.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtdlxumglw.html

for (i in 1..10) println(i)
来源：http://hz.yj20258888.top/gtitwifwsn.html

[T15] Kotlin：接口
来源：http://hz.jqgfzy.top/gtoaruxukt.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtcjukytdt.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gtsfszwcvu.html

print("Hello")
来源：http://hz.cheryme.top/gtjobmbzsz.html

[T17] Swift：变量与常量
来源：http://hz.chenjidiqi.icu/gtbmewhthg.html

var a = 1;  let b = 2
来源：http://hz.hfpthk.cn/gtoxvdauun.html

[T18] Swift：字符串插值
来源：http://hz.cdnleiting.top/gttevowmib.html

"值: \(b)"
来源：http://hz.xuetiantiany.cn/gtzgipyzic.html

[T19] Swift：可选绑定
来源：http://hz.jyoumei.cn/gtpjdithli.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gtnlesxckx.html

[T20] Swift：数组操作
来源：http://hz.dashuyun.cn/gtfkvgavjx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj202588.top/gtfkyxwcjk.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtvbytumgd.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtkfzgunyu.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gtjwifrbww.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258888.top/gtqibnahaj.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtgdmtyqhs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daxiang520.top/gtsbjkbeev.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gteqkrpjet.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hongshengwenyu.top/gtqtocgjmt.html


<!-- 参考信息 -->