代发 wailian999

echo "${#s}"
来源：http://hz.sysykeji.top/gtmhbdnfzt.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtgiwjhftq.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gthihwervk.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtytrkchpv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtdaomtqpi.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtkahulbml.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gthaznxxvp.html

[R25] 去后缀 / 去前缀
来源：http://hz.sxryk.cn/gtycghtsbr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuanzx.com/gtthjxjakh.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtraxrnjrg.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtuubgvsms.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtsayfdwad.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258888.top/gtllgqyvam.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtwfplaehf.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gtjrgdcgkp.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gtdygxzkzs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtmgaekdiz.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gteprfqwzm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ivvv.top/gtzyjwtazn.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtpwydsztx.html

f() { local x=1; echo "$x"; }
来源：http://hz.xziqi.cn/gtilqkxfzo.html

[R32] 参数个数校验
来源：http://hz.yonumen.top/gtlpcnjgee.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtkicmzbxl.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtkdasgara.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258.top/gtvqlyerkj.html

[R34] 退出时清理
来源：http://hz.guannengcc.top/gtotptpgqh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtmxdngxvn.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gtawxxayza.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gthlyecyvv.html

[R36] 并发执行多个任务
来源：http://hz.xziqi.cn/gtncvxbozr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangshuangyany.cn/gtgcrbnhte.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtlmunyonc.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtfqkjgyzk.html

[R38] 管道串联
来源：http://hz.jqgfzy.top/gtafjgmdch.html

cat a.txt | grep -i error | wc -l
来源：http://hz.0kj1m.cn/gtlfmtenzt.html

[R39] 重定向标准输出与错误
来源：http://hz.nwbrower.top/gthbfxgypo.html

cmd > out.log 2>&1
来源：http://hz.zdqjudy.top/gtrolhqwrl.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gttnmihreq.html

echo "log" >> out.log
来源：http://hz.chenzaomai.com/gtsnolnnee.html

[R41] 丢弃输出
来源：http://hz.redwolf501.top/gtzaxtklvp.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtduvnzbmw.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gtdeyhysof.html

wc -l < a.txt
来源：http://hz.zhongyouzk.top/gtdfcdlyqw.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtvnhhrrun.html

find . -name "*.log" -type f
来源：http://hz.cucudq.cn/gtulvlpnob.html

[R44] 按修改时间查找
来源：http://hz.aizwys.cn/gthvwxfwnt.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtbpesqjzu.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtdcwvqlwq.html

find . -name "*.tmp" -delete
来源：http://hz.pycfn.com/gtufegodti.html

[R46] 递归替换文件内容
来源：http://hz.xinyue.icu/gtsqlvljlk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtiyrvbwyh.html

[R47] sed 单行替换
来源：http://hz.cucudq.cn/gtssmbgvbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtkmztjtse.html

[R48] awk 取指定列
来源：http://hz.yanxiufei.cn/gttajeiqwl.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtqukyjvxz.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtrbtbgwzs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gtremujfgw.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gteymrngek.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pycfn.com/gthckgrwtb.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gtlbymxfnp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtqeezjbjj.html

[R52] 统计行数
来源：http://hz.aibaodan.cn/gtcxbuwvnm.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtagimzmux.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtfssnnpum.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtdmijndyu.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gtravpdiil.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtqyreysea.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtgmcmyoyi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtqxiqqmro.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtmlecwqnr.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtdlnnmbku.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtfazmriec.html

ssh user@host 'uptime'
来源：http://hz.fzhhl.top/gtigmksmvl.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtaehckykj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shuidangran.top/gthoxursmo.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtagdmrush.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sweek.top/gtidmphyid.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtylsbuqav.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtdynejjwj.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtubqvknhb.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gtxxlyeoze.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gtvncnyitj.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtblbxewwd.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtnthvrnju.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtyhtcszjl.html

[R64] 结束进程
来源：http://hz.vqdsnc.cn/gtjssbnnwy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gtrepekjvm.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtborkcchm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtodrfptnq.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtdpbdrgpo.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtngkscplt.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gthdfzbhcw.html

openssl rand -hex 16
来源：http://hz.jinqigfzy.top/gtryarlmrl.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gtkavuseis.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtookeopwb.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtyinyyabj.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtpljeibnh.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gtlaeaqjux.html

date +%s;  date -d @1700000000
来源：http://hz.sufxvd.cn/gthkggivre.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtfpccfuzs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gteelxxqdj.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtodyklhbs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sysykeji.top/gttwlsdauo.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtpdxeiwqi.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtyjnwwdoh.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gtyusdvyxx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cucudq.cn/gtwzctxwxq.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtydfnirnh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ywan-chungtsiang.top/gtuprjnpac.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gteplrmcht.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtnrgzqjbk.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangkeji.top/gtkngbixze.html

read -rp "请输入: " ans
来源：http://hz.nanxuanxn.top/gtgizjxfah.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtfonwdqoa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtfzrkpneg.html

[R79] 解析命令行选项
来源：http://hz.daria6918.cn/gtcoqrizih.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtzzyqkgbj.html

[R80] 查看脚本执行耗时
来源：http://hz.hnqzz.top/gtdfswvvga.html

time ./run.sh
来源：http://hz.xinyue.icu/gtbdhpoodd.html

================================================================================
来源：http://hz.zycfv.cn/gtglzpcwav.html

S. C / C++ 专题
来源：http://hz.c1oappe.top/gtjnytvoup.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtveirimea.html

[S01] C：Hello World
来源：http://hz.ivvv.top/gtfemjfyvp.html

#include <stdio.h>
来源：http://hz.guowangkeji.top/gtdegenacs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtaflegueb.html

[S02] C：变量与格式化输出
来源：http://hz.redwolf501.top/gtkmpmaojv.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinyuanbaomall.cn/gtppcbzgeo.html

[S03] C：读入整数
来源：http://hz.sweek.top/gtevrtzttc.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtujfpbzpw.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtqafhvexg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gthcbioprm.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtziaaltof.html

strlen(s)
来源：http://hz.jinqigufen.top/gtapbucuyy.html

[S06] C：字符串比较
来源：http://hz.guannengcc.top/gtyvysyydv.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtlenifucj.html

[S07] C：数组遍历求和
来源：http://hz.zdqjudy.top/gtrytghrzo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgfzy.top/gtalshvowy.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtnqjvcdwx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.c1oappe.top/gtynuvyzbx.html

[S09] C：结构体定义与初始化
来源：http://hz.haohaochexian.top/gtrhqmdnus.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtsgjajsus.html

[S10] C：指针与解引用
来源：http://hz.tianlin.xyz/gtqbuyaotw.html

int *p = &a;  *p = 5;
来源：http://hz.hywenlv.cn/gtstbtfmry.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtnnzjebxc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtkkalyftv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtuypxklto.html

fclose(f);
来源：http://hz.yueranfly.top/gtcckpfbds.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtxrhwnyck.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.smart0.xyz/gtafmnxoow.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtygupiosb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gaohongyu789.top/gtkpdyjzpt.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtxshnvgqe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtvepaogiq.html

[S15] C：类型转换
来源：http://hz.yuanzhike.top/gtvzekggli.html

(double) a / b
来源：http://hz.jinqigfzy.top/gtohzlciob.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtnomrhrlb.html

x |= (1 << 3);
来源：http://hz.kuanghao11.cn/gtlffwpvkc.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gtinrgvjtw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtiphoyjsn.html

[S18] C：命令行参数
来源：http://hz.smart0.xyz/gtscmgeqwm.html

int main(int argc, char **argv)
来源：http://hz.gogol.net.cn/gtoueetafp.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtzdgviszb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtnfgkpxgi.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gttvehuhia.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtjstojvzo.html

[S21] C：字符类别判断
来源：http://hz.yvedp.cn/gtwihewvlh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gtajokojdw.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtiivrljoj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtefnrhbls.html

[S23] C：随机数
来源：http://hz.cheryme.top/gtbjbjcscz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtnufpaexm.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtuzynggsv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydzc1.top/gtxborqaei.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtcnaprmei.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangtech.top/gtdlnaaime.html

[S26] C：内存清零
来源：http://hz.jiagoushi.top/gtspiqlclw.html

memset(a, 0, sizeof a);
来源：http://hz.ywan-chungtsiang.top/gtpwnpyinl.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtutaptazb.html

const double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtwtermwfe.html

[S28] C：静态变量
来源：http://hz.tianlin.xyz/gttilnlcqf.html

static int counter = 0;
来源：http://hz.yj20258.top/gtmkwzxjhy.html

[S29] C：变参函数
来源：http://hz.yongpay.top/gttopcqdvg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtnxnlhemt.html

[S30] C：头文件保护
来源：http://hz.xylfe.cn/gtcmitljpu.html

#ifndef X_H
来源：http://hz.iojbl.cn/gttnyoiktw.html

#define X_H
来源：http://hz.aibaodan.cn/gtmukfetaa.html

#endif
来源：http://hz.cheryme.top/gtbmhcgofq.html

[S31] C++：Hello World
来源：http://hz.ybcxt.top/gtltxhpcgy.html

#include <iostream>
来源：http://hz.hnqzz.top/gtpasgjwhm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hywenlv.cn/gtbepgllao.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gtysrxfvho.html

std::string s = "hi";  s += "!";
来源：http://hz.bjfxy.top/gtxskygcnq.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtyixjujjx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinghuilouyu.cn/gtmbmsbcgk.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtvlmveism.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sweek.top/gtdtkybbeh.html

[S35] C++：map
来源：http://hz.sweek.top/gtekgfzstu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtqzpavigg.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtteubrrle.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtxlltwfdf.html

[S37] C++：set
来源：http://hz.xinyue.icu/gtvzgjehcz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtxfpbnqnc.html

[S38] C++：排序
来源：http://hz.fzhhl.top/gtejzrawrl.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtfkhosowc.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtitngadal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hongshengwenyu.top/gtttnlytvh.html

[S40] C++：查找元素
来源：http://hz.tianlin.xyz/gtlhrvldym.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gtjrpityvi.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gthlrjkovm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gtvxyyabos.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtwtjyhiao.html

class B : public Base { public: void f() override {} };
来源：http://hz.guowangkeji.top/gtxnokisxa.html

[S43] C++：智能指针
来源：http://hz.yuxming.cn/gtmpszjrwv.html

auto p = std::make_unique<int>(5);
来源：http://hz.yongpay.top/gtfdrjgymp.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtinkiwbjz.html

void inc(int &x) { ++x; }
来源：http://hz.chenlongwang.top/gtxewbjxce.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtcqfhmuen.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtvzbskkka.html

[S46] C++：函数模板
来源：http://hz.yangfankeji.com/gtrpuptvjw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtsmitmiuu.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtwpcwbakh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtpaoaofpk.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtcaoelnlo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gtoztdtidz.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtzvosjkya.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtchgpsxpg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtfvmdjpmk.html

[S50] C++：格式化数字
来源：http://hz.daria6918.cn/gtqzofpnya.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtohssnylc.html

[S51] C++：显式类型转换
来源：http://hz.0kj1m.cn/gtsjzffttv.html

static_cast<double>(a) / b
来源：http://hz.gaohongyu789.top/gtkkrognjp.html

[S52] C++：const 与 noexcept
来源：http://hz.chenjidiqi.icu/gtnqpuvfry.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigufen.top/gtmxmivcyg.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtnnwrzpbd.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtvwkrwbnx.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtedjexnmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtnluomajx.html

[S55] C++：结构化绑定
来源：http://hz.chenlongwang.top/gtzbiwxzwf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtkhawzenl.html

[S56] C++：optional
来源：http://hz.tian-w.cn/gtdckwozxq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gttfjrncnr.html

[S57] C++：编译期常量
来源：http://hz.cheryme.top/gtiyvxdlmc.html

constexpr int N = 10;
来源：http://hz.svipenyu.cn/gtmnlrutoh.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtrqcsxcun.html

namespace ns { int f() { return 1; } }
来源：http://hz.smart0.xyz/gtijaduedf.html

[S59] C++：静态断言
来源：http://hz.aizwys.cn/gtcdgmkkoe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtupenhtju.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtgiynthlr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gtwjtuzhjg.html

================================================================================
来源：http://hz.haohaochexian.top/gtxpdmdknt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gtoztotxpk.html

================================================================================
来源：http://hz.guowangkeji.top/gtyreiazox.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtqwyomlwg.html

println("Hello")
来源：http://hz.yvedp.cn/gtoklavqox.html

[T02] Kotlin：变量
来源：http://hz.fengsongda.top/gtadljmifu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtfqgzdusp.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gthtzunzwx.html

"值: $b"
来源：http://hz.daxiang520.top/gtgwkqanxd.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gtjqgwftzt.html

val n: String? = null;  n?.length
来源：http://hz.0kj1m.cn/gtiyggwoem.html

[T05] Kotlin：when 表达式
来源：http://hz.jlsjyb.cn/gtyyrpkmly.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtcwniahgo.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtitzhdodx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gtfbqikwop.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigufen.top/gtqzuzeuge.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sxryk.cn/gtqcmjmeuy.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtcogjnyev.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtutxjjcit.html

[T09] Kotlin：扩展函数
来源：http://hz.iojbl.cn/gtubxpztxa.html

fun String.exclaim() = this + "!"
来源：http://hz.9152youxi.cn/gtrybbhqly.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtunhwzehd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gtcuynsjij.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtrwkywjye.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtzncthuvd.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtuwgyusty.html

val (a, b) = Pair(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtuvicywco.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxinkj.top/gteqfrpdhs.html

val m = mapOf("a" to 1)
来源：http://hz.gotoacloud.top/gtdoeqmgsw.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gthypkapze.html

for (i in 1..10) println(i)
来源：http://hz.zhengqikj.top/gtaxisbmvw.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtnbopafnc.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtakibhyhl.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtwmfhkqcq.html

print("Hello")
来源：http://hz.yueranfly.top/gtmbxxeykj.html

[T17] Swift：变量与常量
来源：http://hz.jqgfzy.top/gtdyxvyvhy.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtzvowjknq.html

[T18] Swift：字符串插值
来源：http://hz.vqdsnc.cn/gthejfgjdp.html

"值: \(b)"
来源：http://hz.ywan-chungtsiang.top/gtszyyjjcr.html

[T19] Swift：可选绑定
来源：http://hz.iojbl.cn/gtgnkxjila.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gtaebhgxym.html

[T20] Swift：数组操作
来源：http://hz.quarkkingdee.top/gthmwbjfee.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gaohongyu789.top/gtffrbslag.html

[T21] Swift：遍历
来源：http://hz.yuanzhike.top/gtqqotaebk.html

for x in a { print(x) }
来源：http://hz.redwolf501.top/gtdgkbsoug.html

[T22] Swift：字典
来源：http://hz.hnqzz.top/gtpeiirafk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhixingplan.top/gtqhcxqccz.html

[T23] Swift：函数
来源：http://hz.snrcjt.cn/gtbvohwrps.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtpphkdwrm.html

[T24] Swift：闭包
来源：http://hz.shangyingyoupin.top/gthcwpazuo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shuidangran.top/gtvmqqwubp.html


<!-- 参考信息 -->