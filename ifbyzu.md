代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.snrcjt.cn/gthbvvhcvb.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtljjbdeyy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gtunykpiyz.html

[R25] 去后缀 / 去前缀
来源：http://hz.jiagoushi.top/gtdkybntfe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenlongwang.top/gtxptnyroe.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtjslvjfjk.html

now=$(date +%F); echo "$now"
来源：http://hz.gotoacloud.top/gteoeoxary.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtaehqdrtt.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtoexgbddi.html

[R28] 浮点运算
来源：http://hz.jinghuilouyu.cn/gtqwoyausv.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gtzsohrcyi.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtulwsfeep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gogol.net.cn/gtczqkmnie.html

[R30] 函数返回状态码
来源：http://hz.aizwys.cn/gtzbamwgmp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtsjdaykab.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtokiyzimk.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj202588.top/gtesmupjsm.html

[R32] 参数个数校验
来源：http://hz.cucudq.cn/gttsnghipd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigufen.top/gtscxsufzu.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtzqkhpxez.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gtelphfhaw.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtogthgruj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtgrtwtvtc.html

[R35] 后台执行并等待
来源：http://hz.9152youxi.cn/gtcehwwnie.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gttqsoqhwl.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtzymxytlq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xingfuxueyuan.xyz/gteaxhqvyf.html

[R37] 把输出赋给变量
来源：http://hz.316326.xyz/gtoolhffle.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtfapbvmec.html

[R38] 管道串联
来源：http://hz.jlsjyb.cn/gtgwuhnguz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtspwdkscn.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtsjwqpnwo.html

cmd > out.log 2>&1
来源：http://hz.tianlin.xyz/gtddryqzys.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtoaeuuvwf.html

echo "log" >> out.log
来源：http://hz.zdqjudy.top/gtfrnosdkm.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtcegqrlun.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtxafcgfjd.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gtqcldaqmp.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtlhnsqyru.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gteyuwaqwn.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtcszewfkv.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtshgqffsm.html

find . -mtime -7 -type f
来源：http://hz.jinqigufen.top/gtbjrmrorn.html

[R45] 批量删除
来源：http://hz.zycfv.cn/gtmxjgvagq.html

find . -name "*.tmp" -delete
来源：http://hz.redwolf501.top/gthdrrzpzg.html

[R46] 递归替换文件内容
来源：http://hz.meibo888.top/gtxvmwimfu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gotoacloud.top/gtudsbciyp.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtiegateeg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtiiyqvoom.html

[R48] awk 取指定列
来源：http://hz.feifeiyinyue.top/gtzohjagwg.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtgaalejue.html

[R49] awk 带条件
来源：http://hz.bjfxy.top/gtetkocfrz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gttdquonfq.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtapnmhdqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daria6918.cn/gtaeafwpdw.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtqzgtmpli.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xziqi.cn/gtdjgvrmjp.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gthwfeqwti.html

wc -l a.txt
来源：http://hz.chenjidiqi.icu/gtqvkulmtr.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtpzaxqunu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtqbebbygu.html

[R54] 比较两个文件
来源：http://hz.sxryk.cn/gtgrhzpwkt.html

diff a.txt b.txt
来源：http://hz.xuetiantiany.cn/gtjpxyulzh.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtjjfsqtzs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gtmmtfkulq.html

[R56] 远程拷贝
来源：http://hz.haohaochexian.top/gtqammvrrk.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtlbtsdhmg.html

[R57] 远程执行命令
来源：http://hz.dianchejie.cn/gthrcravef.html

ssh user@host 'uptime'
来源：http://hz.tanke756.top/gthnhdhrwx.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtwhjuclyo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuetiantiany.cn/gtptxdixay.html

[R59] 发 POST JSON
来源：http://hz.hnxiangtu.top/gtuvtmywmt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.316326.xyz/gtovviqvdm.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuanzx.com/gtzxzvemsf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pycfn.com/gtdswhonrn.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtjitkgrjo.html

df -h;  du -sh *
来源：http://hz.ydzc1.top/gtnbtgxgxd.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gtpyblslxw.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtuossrirp.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtttwayfef.html

free -h;  ps aux | grep nginx
来源：http://hz.9152youxi.cn/gtwsizmqxd.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtbkguzsdv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtrvmowuif.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtwhlfuusq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hysaishi.cn/gtbojwaufw.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtolmurtuw.html

crontab -e;  crontab -l
来源：http://hz.daxiang520.top/gtcgxbcqwt.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigfzy.top/gtplhvhzpl.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtxaobfmoz.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtmpiccbvm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtyzjvdxab.html

[R69] 生成随机密码
来源：http://hz.zhoulong.xyz/gtyslrxuxn.html

head -c 16 /dev/urandom | base64
来源：http://hz.dianchejie.cn/gtmwomepxe.html

[R70] 时间戳与互转
来源：http://hz.mhx1999.top/gtibxcyesk.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtxvzqlrtc.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtvjsdgobk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgufenzy.top/gtsozisbrg.html

[R72] 等待端口就绪
来源：http://hz.chenlongwang.top/gtfccppegg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gogol.net.cn/gtopqeerej.html

[R73] 分割大日志
来源：http://hz.sysykeji.top/gtaghrtsbg.html

split -l 1000 big.log part_
来源：http://hz.andypj.xyz/gtkusfkepk.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtqskhzysv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nwbrower.top/gtxbbtryps.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtkksczszm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gttjjxcrjh.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtlzdzugnb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtxdpfbgwn.html

[R77] 读取用户输入
来源：http://hz.fengsongda.top/gtnivedzrh.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtprywsxzn.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtqdrohfcd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtsvokqhgj.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtvsagzrum.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtzaxepvgx.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtxtykmbmr.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtcmtcjhwr.html

================================================================================
来源：http://hz.zhengqikj.top/gteladxpkg.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtbshrcobl.html

================================================================================
来源：http://hz.gogol.net.cn/gtdswnfujg.html

[S01] C：Hello World
来源：http://hz.pengpengdd.cyou/gtqeewofui.html

#include <stdio.h>
来源：http://hz.cucudq.cn/gtqvayunqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gogol.net.cn/gtmgrvrhze.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtcnnyngtc.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtowprghbn.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtzkquhxju.html

int x; scanf("%d", &x);
来源：http://hz.shangyingyoupin.top/gtohmxykxs.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtpztquyih.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtiztwbshc.html

[S05] C：字符串长度
来源：http://hz.nanxinkj.top/gtjuahwlwb.html

strlen(s)
来源：http://hz.cheryme.top/gtmwqgeyfx.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gtjolpdhii.html

strcmp(a, b) == 0
来源：http://hz.tian-w.cn/gtmzqvbfrj.html

[S07] C：数组遍历求和
来源：http://hz.dianchejie.cn/gtexnrbfdm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuanzhike.top/gttcrevjhj.html

[S08] C：动态内存分配与释放
来源：http://hz.xinyue.icu/gtozhalgdj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtqwvjcwcu.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtjhkukcgs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gtzcbqipcq.html

[S10] C：指针与解引用
来源：http://hz.zhaomingkeji.xyz/gtgobjfkow.html

int *p = &a;  *p = 5;
来源：http://hz.52xcode.cn/gtqqmpixir.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtlqiwpiks.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yanxiufei.cn/gtaioxxbxe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hammf.cn/gtlrzlvxsn.html

fclose(f);
来源：http://hz.jlsjyb.cn/gtsgvsbyen.html

[S12] C：写文件
来源：http://hz.aibaodan.cn/gtlfgwdkba.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtlxtndubf.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gtyfypxlps.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtkblwkdtn.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtlkcsryha.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xinyue.icu/gtvykeuudz.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gtfkpvlczv.html

(double) a / b
来源：http://hz.ydzc1.top/gtitgacgvo.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gthehchgdk.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtixjbtgdq.html

[S17] C：安全拼接字符串
来源：http://hz.9152youxi.cn/gtvrlhpdsc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhaomingkeji.xyz/gtcdrrdjdg.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gtczwydvbw.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtqadkmvtv.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gthnlberyi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtaueizrrw.html

[S20] C：二分查找
来源：http://hz.havefunace.top/gtrwoewneo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtzcjeecad.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtrnnuvqob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cdnleiting.top/gtgwnkqjfk.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtqvikxpyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sufxvd.cn/gtobtycjaf.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtaexfbgad.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtvjwrarcx.html

[S24] C：获取本地时间
来源：http://hz.hnqzz.top/gtchmzwxxl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gtfokqlffn.html

[S25] C：内存拷贝
来源：http://hz.ybcxt.top/gtfmnnfgdn.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtobkzofcy.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtgmxxejjn.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtnabssezf.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtxflosgkz.html

const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtflwdtpre.html

[S28] C：静态变量
来源：http://hz.pengpengdd.cyou/gtmjkcjvhk.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtqgjarmfn.html

[S29] C：变参函数
来源：http://hz.gogol.net.cn/gtafswhidh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cucudq.cn/gteulrpcre.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtdbfhopqj.html

#ifndef X_H
来源：http://hz.cdnleiting.top/gtkyrlmziz.html

#define X_H
来源：http://hz.shuidangran.top/gtniccancw.html

#endif
来源：http://hz.yj20258888.top/gtkffmevmr.html

[S31] C++：Hello World
来源：http://hz.sweek.top/gtvqaexijy.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gtqiaorgxm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gtboberkdk.html

[S32] C++：字符串
来源：http://hz.daxiang520.top/gtoselhguh.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtntelalzz.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtkxngcdne.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.0kj1m.cn/gtnqhettal.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtkkmtolxw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gturdqtutb.html

[S35] C++：map
来源：http://hz.nanxuanxn.top/gtohxtwenw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtxnipdyqa.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gthsyklcds.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtcbvpkxsg.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtjnxpubeh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.bjfxy.top/gtebeemthz.html

[S38] C++：排序
来源：http://hz.jinqigufen.top/gtvhuenqxa.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtfwutmwgn.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtvityydrk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangkeji.top/gtsarndqyd.html

[S40] C++：查找元素
来源：http://hz.quarkkingdee.top/gtkdwhggeq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtyxikymsh.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gtdrtmtaht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gteiycvvin.html

[S42] C++：继承与虚函数
来源：http://hz.c1oappe.top/gtfunqudvb.html

class B : public Base { public: void f() override {} };
来源：http://hz.gogol.net.cn/gtagezlpgu.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtbtaqzysy.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtxyzcxnxz.html

[S44] C++：引用传参
来源：http://hz.pycfn.com/gttalulqru.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtjgglpxds.html

[S45] C++：lambda
来源：http://hz.ydjk.org.cn/gtjlviyvio.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jyoumei.cn/gttgziizih.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtedkwwczi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxinkj.top/gtusmdtwer.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangtech.top/gtipukyjxt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fzhhl.top/gtaoecmysh.html

[S48] C++：逐行读文件
来源：http://hz.chenjidiqi.icu/gthfijywvw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtfdfeiksp.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigufen.top/gtmvmamjnc.html

[S49] C++：写文件
来源：http://hz.cdnleiting.top/gtmscdvevc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtwjulqqql.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtozgjlpea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gtexvqbmfc.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gtdaetpzvd.html

static_cast<double>(a) / b
来源：http://hz.hfpthk.cn/gtgdpnabyu.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtlncpiuju.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtfkfvkwkb.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtowwxfrsg.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtfhvjqgwn.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gtlpxnbrxe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xinyue.icu/gtekfkfnfw.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gthfpmdoqr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtdvnduxvj.html

[S56] C++：optional
来源：http://hz.guowangkeji.top/gtxzbcqxbt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangtech.top/gtnyohpsya.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gtjbjxdify.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtrkukpspm.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtazgzpywp.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangshuangyany.cn/gtgzbvugge.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtuchzpeqp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cdnleiting.top/gtoaaecbau.html

[S60] C++：遍历并删除元素
来源：http://hz.hnxiangtu.top/gtsovoxngm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtplyppeci.html

================================================================================
来源：http://hz.jinqigfzy.top/gttbmdytkx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtwtxaabek.html

================================================================================
来源：http://hz.52xcode.cn/gtfpokiwmj.html

[T01] Kotlin：Hello World
来源：http://hz.sxryk.cn/gtubxzucvc.html

println("Hello")
来源：http://hz.zhengqikj.top/gttyvajqrq.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtyaoskgij.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gotoacloud.top/gtbqjswktp.html

[T03] Kotlin：字符串模板
来源：http://hz.ydjk.org.cn/gtwzqqagkc.html

"值: $b"
来源：http://hz.52xcode.cn/gtjyckqqbl.html

[T04] Kotlin：空安全
来源：http://hz.iojbl.cn/gtpnktgynq.html

val n: String? = null;  n?.length
来源：http://hz.xylfe.cn/gtvdvumqcf.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtakzmprbd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cqqwz.cn/gtsebjltmf.html

[T06] Kotlin：集合映射
来源：http://hz.snrcjt.cn/gtlqzkotcj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydzc1.top/gtsnbnrsty.html

[T07] Kotlin：集合过滤
来源：http://hz.meibo888.top/gtzsaksfwu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aibaodan.cn/gtpuuepijk.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtaljphhpo.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtnmwszrrn.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gtzsxkarst.html

fun String.exclaim() = this + "!"
来源：http://hz.chenjidiqi.icu/gtgqpouikw.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtraulxamy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtiqgzbpfk.html

[T11] Kotlin：协程
来源：http://hz.gogol.net.cn/gtfmqynfht.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtvhlxgxof.html

[T12] Kotlin：解构声明
来源：http://hz.pengpengdd.cyou/gtpuzjuxwb.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtljfbpkwp.html

[T13] Kotlin：只读 Map
来源：http://hz.bjfxy.top/gtolvrqhmp.html

val m = mapOf("a" to 1)
来源：http://hz.sufxvd.cn/gtmierkbgd.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gtniwuyfel.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtokgfkncq.html

[T15] Kotlin：接口
来源：http://hz.shzxlz.cn/gtnqesqhvl.html

interface Shape { fun area(): Double }
来源：http://hz.jinghuilouyu.cn/gtamaqauzp.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtplmrdbhi.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtonklcfuw.html

[T17] Swift：变量与常量
来源：http://hz.cheryme.top/gtscxaldzc.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gthpjkwxlt.html

[T18] Swift：字符串插值
来源：http://hz.jqgufenzy.top/gtbwgwkrcb.html

"值: \(b)"
来源：http://hz.jianghu66.top/gtytbibwde.html

[T19] Swift：可选绑定
来源：http://hz.zhaomingkeji.xyz/gtcfzpqncw.html

if let n = opt { print(n) }
来源：http://hz.hammf.cn/gthdpxzglx.html

[T20] Swift：数组操作
来源：http://hz.ppjwa.cn/gtyaudkyxt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtdoelmtle.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtdzywbyxq.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtwdpgohxd.html

[T22] Swift：字典
来源：http://hz.9152youxi.cn/gtkueurzgo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangkeji.top/gtslzrfisz.html

[T23] Swift：函数
来源：http://hz.zhiwuduotai.top/gtstspqjta.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtqzawpwwa.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gtugzbzpky.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtaaafkehc.html

[T25] Swift：结构体
来源：http://hz.xingfuxueyuan.xyz/gtqohfsbjd.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gtnavnfmiw.html

[T26] Swift：类与重写
来源：http://hz.zhiwuduotai.top/gthoikpsdm.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gtqtoyeahl.html


<!-- 参考信息 -->