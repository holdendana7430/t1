代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangdashe.top/gtpqnvxzkg.html

[R24] 大小写转换
来源：http://hz.iojbl.cn/gtvnojddfp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtcrngczvq.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj202588.top/gthhdqqjie.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gttutovwip.html

[R26] 命令替换
来源：http://hz.chenzaomai.com/gtevmqfebn.html

now=$(date +%F); echo "$now"
来源：http://hz.xylfe.cn/gtwlwcrbpc.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtdyekrsgx.html

echo $((1 + 2 * 3))
来源：http://hz.dianchejie.cn/gtfwxhxmpv.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtfyejotgy.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtdfgriqmk.html

[R29] 定义函数
来源：http://hz.xylfe.cn/gtobgquxud.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.meibo888.top/gthbycbvbf.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtemlxubwp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gtlksimzur.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtgblsikyq.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtydbovjtm.html

[R32] 参数个数校验
来源：http://hz.ivvv.top/gttsyafmyr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gotoacloud.top/gterfwyvxt.html

[R33] 捕获错误并提示行号
来源：http://hz.redwolf501.top/gtfkexexve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenlongwang.top/gthaaykoei.html

[R34] 退出时清理
来源：http://hz.yonumen.top/gtvnsesfze.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtfybydwjy.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtedddcaxc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gthwwulynu.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gtcwvwqirs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtfgxiezuz.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gtqslmsbhd.html

files=$(ls -1)
来源：http://hz.bjfxy.top/gtncdslzab.html

[R38] 管道串联
来源：http://hz.guowangkeji.top/gttcdhgczv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gthlupltab.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gttotnywlg.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtzboasomj.html

[R40] 追加写日志
来源：http://hz.sxryk.cn/gtysuznycp.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtztlfqhig.html

[R41] 丢弃输出
来源：http://hz.hammf.cn/gtvnujbopg.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gthyvoyjfr.html

[R42] 输入重定向
来源：http://hz.jyoumei.cn/gtummitmnk.html

wc -l < a.txt
来源：http://hz.sysykeji.top/gtwaxsyleo.html

[R43] 按名字查找文件
来源：http://hz.sxryk.cn/gtzxugtgle.html

find . -name "*.log" -type f
来源：http://hz.haohaochexian.top/gtxmkbglhe.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtztdwhxzo.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtlyiyooeh.html

[R45] 批量删除
来源：http://hz.daxiang520.top/gtakptymzx.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtwsvdhzem.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtzgldhswq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtnwjrayli.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtobutrvln.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtykeewnnm.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtdbncexxm.html

awk '{print $1, $3}' a.txt
来源：http://hz.ivvv.top/gtybdaxsff.html

[R49] awk 带条件
来源：http://hz.nanxinkj.top/gtzcllvasc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ivvv.top/gtlpbnzaea.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gtifbxbfky.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fengsongda.top/gtpqsbsvhm.html

[R51] 排序去重取前几
来源：http://hz.gaohongyu789.top/gtwliebviy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtcxuivzov.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtodcnxmsr.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtwfhpadfc.html

[R53] 查看文件头与实时尾
来源：http://hz.tianlin.xyz/gtkyulvkuz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtqsjiaqsc.html

[R54] 比较两个文件
来源：http://hz.cashguo.top/gtgqhulsrv.html

diff a.txt b.txt
来源：http://hz.yangfankeji.com/gtgcecfjdt.html

[R55] 压缩与解压
来源：http://hz.aibaodan.cn/gthomicuwv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtghmrucso.html

[R56] 远程拷贝
来源：http://hz.gzhubu.top/gtqmohkqos.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gteipkzbex.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtncrrnquc.html

ssh user@host 'uptime'
来源：http://hz.cashguo.top/gtbpgsaqep.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtcjqhfjpe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtcnbkqnwe.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtxmztfrhe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gtumrennix.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtinncdwaj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtflystgoe.html

[R61] 磁盘占用
来源：http://hz.feifeiyinyue.top/gtmyuoayba.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtsfakfgoz.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gtvpbrfguy.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtjzbxvztd.html

[R63] 内存与进程
来源：http://hz.jlsjyb.cn/gtzlltcznu.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangtech.top/gtivektrhr.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtzsixilkl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gteftjttbm.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtvpxnqloa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtejqqkvlg.html

[R66] 定时任务
来源：http://hz.pycfn.com/gtglayufom.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtvipjehxr.html

[R67] 生成随机十六进制串
来源：http://hz.hammf.cn/gticzwmvhh.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtnbxledbe.html

[R68] 计算文件校验值
来源：http://hz.chenlongwang.top/gtqjxuawsl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtwqrnemsz.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtuajyctgi.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtdruqvahk.html

[R70] 时间戳与互转
来源：http://hz.fengsongda.top/gtannynccj.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtfzpytyrc.html

[R71] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtuzfopsga.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtinjqtbii.html

[R72] 等待端口就绪
来源：http://hz.shzxlz.cn/gtsqmfurce.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gtffxbshso.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtdinoifma.html

split -l 1000 big.log part_
来源：http://hz.0kj1m.cn/gtxdscscfd.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gtxmyptins.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cashguo.top/gtblqxidzd.html

[R75] 导出环境变量
来源：http://hz.hfpthk.cn/gtclljtzya.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtgceapzoo.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtrdfvocpi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtewmswtot.html

[R77] 读取用户输入
来源：http://hz.svipenyu.cn/gtmrasjpsf.html

read -rp "请输入: " ans
来源：http://hz.nwbrower.top/gtjwpjpqja.html

[R78] 交互式菜单
来源：http://hz.tanke756.top/gtjcagxumc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sysykeji.top/gtyodyxnkd.html

[R79] 解析命令行选项
来源：http://hz.snrcjt.cn/gtsetgojid.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guannengcc.top/gtprcdykyb.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258.top/gtmpvgmurr.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtwdwfgcep.html

================================================================================
来源：http://hz.hammf.cn/gtbqayibet.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtqsmhegce.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvympoexn.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtxskuhejf.html

#include <stdio.h>
来源：http://hz.jlsjyb.cn/gttgtmsewd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hammf.cn/gtthqiksll.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gtqlcbjxsb.html

int a = 10; printf("%d\n", a);
来源：http://hz.fengsongda.top/gtgoenyvov.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gthwwxhjzr.html

int x; scanf("%d", &x);
来源：http://hz.ywan-chungtsiang.top/gtvjejgwkw.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gtyntyatgt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtzkaacmxd.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtzyxjvyby.html

strlen(s)
来源：http://hz.zhaomingkeji.xyz/gtdkccirez.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtrtyksybc.html

strcmp(a, b) == 0
来源：http://hz.cashguo.top/gthorjqmby.html

[S07] C：数组遍历求和
来源：http://hz.ivvv.top/gtgniinvyr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.havefunace.top/gtyyluntoh.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtsxazeneu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.c1oappe.top/gtfebrmwdm.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtlixzpffg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtswfiavjp.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gttyqqelur.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gtcxbjxoau.html

[S11] C：逐行读文件
来源：http://hz.sysykeji.top/gtjmlhunty.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.havefunace.top/gtkrfojqxz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gtsyspanlq.html

fclose(f);
来源：http://hz.daria6918.cn/gthtgrwyyx.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtthqskcka.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gthwnepacy.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gthoszdzhr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gttbonyosq.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtmrigwxvc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtjqwnttli.html

[S15] C：类型转换
来源：http://hz.hysaishi.cn/gtbclesppe.html

(double) a / b
来源：http://hz.sxryk.cn/gtgwpaofcu.html

[S16] C：位操作置位
来源：http://hz.zhengqikj.top/gtfcnghefs.html

x |= (1 << 3);
来源：http://hz.0kj1m.cn/gtqhindzex.html

[S17] C：安全拼接字符串
来源：http://hz.pengpengdd.cyou/gtxoldzpkh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenzaomai.com/gtkcniincp.html

[S18] C：命令行参数
来源：http://hz.redwolf501.top/gtwwjksreu.html

int main(int argc, char **argv)
来源：http://hz.9152youxi.cn/gtygilrtni.html

[S19] C：快速排序
来源：http://hz.daria6918.cn/gtxlfndben.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtvflrgzca.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtcvjsqdaq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtrjmdqvby.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gtqavkezug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.mhx1999.top/gtzmbhftjf.html

[S22] C：字符串转数字
来源：http://hz.cashguo.top/gthebxvgoz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnqzz.top/gtcfgyltje.html

[S23] C：随机数
来源：http://hz.yj202588.top/gtntqsagpa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tian-w.cn/gtgybujizg.html

[S24] C：获取本地时间
来源：http://hz.ydjk.org.cn/gtcbiegvyt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtkfccxbhp.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtpwcfnszi.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtcdhutmxi.html

[S26] C：内存清零
来源：http://hz.smart0.xyz/gtoledrlgz.html

memset(a, 0, sizeof a);
来源：http://hz.ybcxt.top/gtoewvqkhq.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtejmnjtck.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtzmyaakwt.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtwbxxjlyc.html

static int counter = 0;
来源：http://hz.cheryme.top/gtqkilxvic.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtvltmzsit.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtdhdepjvm.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtgxkysuqi.html

#ifndef X_H
来源：http://hz.jiagoushi.top/gtnvjabqqj.html

#define X_H
来源：http://hz.hnqzz.top/gtfocqdeyu.html

#endif
来源：http://hz.xinyue.icu/gtvjnigplp.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtaocllkci.html

#include <iostream>
来源：http://hz.aizwys.cn/gtwaxrywwe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258.top/gtetiunznz.html

[S32] C++：字符串
来源：http://hz.zhiwuduotai.top/gtxzcvnewt.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtjfsuejtf.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtapvnfpro.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtjbtkoesc.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtxidjtqzh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtiijssvsh.html

[S35] C++：map
来源：http://hz.sxryk.cn/gttgbicjuf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtwyhwkvjy.html

[S36] C++：unordered_map
来源：http://hz.tian-w.cn/gtgbbzaghq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guowangkeji.top/gtvdoxjujf.html

[S37] C++：set
来源：http://hz.nanxuanxn.top/gtlwkavpsf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtrokvwvry.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtldnbilni.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gtkdusqvfm.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtnrvguvlt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtneqyoovz.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gtzivpnsob.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yonumen.top/gtynfjddfa.html

[S41] C++：类与构造函数
来源：http://hz.andypj.xyz/gtkabgpmcr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gteelstkzq.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtplevbnlf.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtjnlpanij.html

[S43] C++：智能指针
来源：http://hz.havefunace.top/gtzfkzooej.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinqigfzy.top/gtlddyvglh.html

[S44] C++：引用传参
来源：http://hz.feifeiyinyue.top/gtwbluojyd.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gthqlmfyxc.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gthotoiroj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhongyouzk.top/gtyotcedxa.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtowcpbydh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtozobpiem.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtzkbdwivd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtxoijabic.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtkyydinua.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtvjzoepeo.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gthbswyrpx.html

[S49] C++：写文件
来源：http://hz.9152youxi.cn/gtjtmzcrzv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tanke756.top/gtieszlmec.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtbtiaufle.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtekneogcd.html

[S51] C++：显式类型转换
来源：http://hz.yonumen.top/gtoragkzya.html

static_cast<double>(a) / b
来源：http://hz.hfpthk.cn/gthapduawk.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gtynbimzsu.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gtfjfmhrrh.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtusnjgqsj.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gthihtyekl.html

[S54] C++：异常处理
来源：http://hz.jqgufenzy.top/gtkdsggdrh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtaxrtkrou.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtzoexmgxj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yangfankeji.com/gtrwpowgto.html

[S56] C++：optional
来源：http://hz.nanxinkj.top/gtehrnwoaa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gtiulokzus.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtfxiuggbn.html

constexpr int N = 10;
来源：http://hz.xingfuxueyuan.xyz/gtrjpltmzh.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtfcirvjsp.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gteprxpayv.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtekvvftqx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj202588.top/gtehrncxxp.html

[S60] C++：遍历并删除元素
来源：http://hz.gogol.net.cn/gtzkohqtbd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xylfe.cn/gteelhhzhp.html

================================================================================
来源：http://hz.xuanzx.com/gtynwfxsdl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yanxiufei.cn/gtjasjxenn.html

================================================================================
来源：http://hz.fzhhl.top/gthtsumgkl.html

[T01] Kotlin：Hello World
来源：http://hz.9152youxi.cn/gtwmjkbolt.html

println("Hello")
来源：http://hz.dashuyun.cn/gtlknywsig.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtjfrwzcen.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.mhx1999.top/gtmtstvaww.html

[T03] Kotlin：字符串模板
来源：http://hz.bjfxy.top/gtnxufaxgz.html

"值: $b"
来源：http://hz.52xcode.cn/gtaykjbpmq.html

[T04] Kotlin：空安全
来源：http://hz.yongpay.top/gtpjweyhvk.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtwcfosuge.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtwvcaeito.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtmmrnpefa.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtyeemzbhh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtotojezda.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gtmlgirbmh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.smart0.xyz/gtbxjvwtnq.html

[T08] Kotlin：数据类
来源：http://hz.c1oappe.top/gtohgnchli.html

data class User(val name: String, val age: Int)
来源：http://hz.iojbl.cn/gtihpbjzot.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtldimdcug.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtlcboavlv.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangkeji.top/gtcseleiks.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dashuyun.cn/gtgqdlhyzw.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtfbrmzcwn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.0kj1m.cn/gtyxzqkwls.html

[T12] Kotlin：解构声明
来源：http://hz.316326.xyz/gtwqkpneqa.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gteyzsyrwk.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtfoacsewr.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtsgevwxxx.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gtxqdywzof.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtkwbrzxcv.html

[T15] Kotlin：接口
来源：http://hz.daria6918.cn/gthvztltze.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtmvjchili.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtplkcackf.html

print("Hello")
来源：http://hz.svipenyu.cn/gtauxugpfd.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtkztmwpll.html

var a = 1;  let b = 2
来源：http://hz.gogol.net.cn/gtohqkbguy.html

[T18] Swift：字符串插值
来源：http://hz.dashuyun.cn/gtsyaaszew.html

"值: \(b)"
来源：http://hz.havefunace.top/gtzguembel.html

[T19] Swift：可选绑定
来源：http://hz.feifeiyinyue.top/gtxqmpczta.html

if let n = opt { print(n) }
来源：http://hz.feifeiyinyue.top/gtdozotkje.html

[T20] Swift：数组操作
来源：http://hz.yj202588.top/gtjhmrriul.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ppjwa.cn/gtxsnixtpb.html

[T21] Swift：遍历
来源：http://hz.fzhhl.top/gtnojbmjzv.html

for x in a { print(x) }
来源：http://hz.chenzaomai.com/gtdmovsmzf.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtodxuvquu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhongyouzk.top/gtiuuwmyiv.html

[T23] Swift：函数
来源：http://hz.wangdashe.top/gthmolgqzh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jiagoushi.top/gtjhkycfxu.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtobhvyjzm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gtwzbvgxxd.html

[T25] Swift：结构体
来源：http://hz.shangyingyoupin.top/gtthfufgzd.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtgeszprkl.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtlkuwqdmx.html

class A: Base { override func f() {} }
来源：http://hz.pycfn.com/gtrtkyqhkr.html


<!-- 参考信息 -->