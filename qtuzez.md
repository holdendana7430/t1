代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sxryk.cn/gtmfyfswus.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtgxihgqek.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gteijxjeik.html

[R27] 算术展开
来源：http://hz.yueranfly.top/gtcujwbeld.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtxluomkvu.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gttynnnxyc.html

echo "scale=2; 10/3" | bc
来源：http://hz.haohaochexian.top/gtapmyxvyn.html

[R29] 定义函数
来源：http://hz.feifeiyinyue.top/gtfbgtdsbd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ybcxt.top/gtbosgsbei.html

[R30] 函数返回状态码
来源：http://hz.jinyuanbaomall.cn/gtrshehsri.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zycfv.cn/gtguntjlgt.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtotzgqfne.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtxfmiuvfk.html

[R32] 参数个数校验
来源：http://hz.tianlin.xyz/gtsfottbgu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hammf.cn/gtbkcyfltf.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtbximiyyz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hfpthk.cn/gtjdnfhsmt.html

[R34] 退出时清理
来源：http://hz.pengpengdd.cyou/gtegggbipl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gthceoijhg.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtiqrhzbkk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtvyoyimxg.html

[R36] 并发执行多个任务
来源：http://hz.smart0.xyz/gtmylblunn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtefdmging.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtbqhzgpiq.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtnbmbpvxs.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtmhigtedm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258.top/gtciawkmpj.html

[R39] 重定向标准输出与错误
来源：http://hz.fzhhl.top/gtjbfherub.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtgjskamjr.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtkffklxzl.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtdmxvmoen.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gttyylzvup.html

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gttxksemvt.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtmgokrlra.html

wc -l < a.txt
来源：http://hz.sufxvd.cn/gtkjjbwagy.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtlticwfos.html

find . -name "*.log" -type f
来源：http://hz.meibo888.top/gtxivefndc.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtrlmooysr.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtghqffutp.html

[R45] 批量删除
来源：http://hz.ydzc1.top/gtydkyltjt.html

find . -name "*.tmp" -delete
来源：http://hz.yueranfly.top/gtigjcmcup.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtgkzldtrn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gtxzuzpsyp.html

[R47] sed 单行替换
来源：http://hz.cucudq.cn/gtpjlcfwzf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.9152youxi.cn/gtgpgwxjwy.html

[R48] awk 取指定列
来源：http://hz.gogol.net.cn/gtrtsxvaez.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtgmxiffpm.html

[R49] awk 带条件
来源：http://hz.jinqigufen.top/gtnvcbbtni.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtqpcnntym.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtogselgfq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigfzy.top/gtkxawsppy.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtzfiqgyfp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtanekpmgr.html

[R52] 统计行数
来源：http://hz.nwbrower.top/gtvkeynqml.html

wc -l a.txt
来源：http://hz.xingfuxueyuan.xyz/gtjtpafpeg.html

[R53] 查看文件头与实时尾
来源：http://hz.cucudq.cn/gtqiktwjjg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ywan-chungtsiang.top/gtyyvivbbt.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtvphficjs.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gteenkqqca.html

[R55] 压缩与解压
来源：http://hz.gogol.net.cn/gtelephpwe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xinyue.icu/gtimxetfbu.html

[R56] 远程拷贝
来源：http://hz.pengpengdd.cyou/gtrobllntv.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gtkgbhvxks.html

[R57] 远程执行命令
来源：http://hz.quarkkingdee.top/gtlalrexaf.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtfdiqmaib.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gtqkaqtyjp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gtelblqpmc.html

[R59] 发 POST JSON
来源：http://hz.hysaishi.cn/gtqgnpbdlq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtewusqlba.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtqupssokr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gteirmzjaq.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtesqbyrbt.html

df -h;  du -sh *
来源：http://hz.jinghuilouyu.cn/gtwfgtbzvj.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gtjlbtksum.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtsealtqyn.html

[R63] 内存与进程
来源：http://hz.quarkkingdee.top/gtdpujrpap.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtvfrhlgoj.html

[R64] 结束进程
来源：http://hz.cashguo.top/gtgajibxnw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtecbqriyu.html

[R65] 查看端口占用
来源：http://hz.meibo888.top/gttgprbgnm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gtwxcvvgka.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtlfywvcmd.html

crontab -e;  crontab -l
来源：http://hz.ehwqpu.com/gtsxpptqgj.html

[R67] 生成随机十六进制串
来源：http://hz.xuetiantiany.cn/gtxqixyfak.html

openssl rand -hex 16
来源：http://hz.hywenlv.cn/gtkdwiwpph.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gttaqeupsb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tian-w.cn/gtmezqebyi.html

[R69] 生成随机密码
来源：http://hz.quarkkingdee.top/gtjvlegcok.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gtwisqbgud.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtzymfcglk.html

date +%s;  date -d @1700000000
来源：http://hz.yongpay.top/gthbkereht.html

[R71] 日期格式化
来源：http://hz.yanxiufei.cn/gtyioabyzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtfqaespuv.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtbmaoghpj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtrchokwam.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtospgzcfn.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtbnkomibm.html

[R74] 批量重命名
来源：http://hz.cqqwz.cn/gttjmsxhki.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gtssajrnbt.html

[R75] 导出环境变量
来源：http://hz.xingfuxueyuan.xyz/gtdxlbibls.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtzgrayioy.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtuopjhrzz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtgajfozlk.html

[R77] 读取用户输入
来源：http://hz.zhengqikj.top/gtkgzwadvy.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtbaqzyind.html

[R78] 交互式菜单
来源：http://hz.snrcjt.cn/gtncothaxd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sufxvd.cn/gtzbnoffvp.html

[R79] 解析命令行选项
来源：http://hz.ehwqpu.com/gtlrwpneuz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gticgpgsfm.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtmncmylhq.html

time ./run.sh
来源：http://hz.tanke756.top/gtgaglmqhw.html

================================================================================
来源：http://hz.yueranfly.top/gtgosembeu.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gtrvyimbby.html

================================================================================
来源：http://hz.sweek.top/gtiirlbqjp.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtytfxnryk.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtmkjdpmyx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gtoaaubvhn.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtcednhsxl.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtbyydvrye.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtakzmxnio.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtwoopulsm.html

[S04] C：字符串复制
来源：http://hz.mhx1999.top/gtxxluukkp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtlixixlip.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gtjpkixmyb.html

strlen(s)
来源：http://hz.ydzc1.top/gtedmcseth.html

[S06] C：字符串比较
来源：http://hz.jianghu66.top/gtdupotocu.html

strcmp(a, b) == 0
来源：http://hz.smart0.xyz/gtspuzkthp.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtvozdmdqh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tianlin.xyz/gttwglzhgj.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtyxwceiyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tanke756.top/gtqrezgmfg.html

[S09] C：结构体定义与初始化
来源：http://hz.zhijiandao.cn/gtrsbrsqpg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtpqrmpqfb.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtpvashkby.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtqpszbsxp.html

[S11] C：逐行读文件
来源：http://hz.sweek.top/gtpwcaaust.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gtwmjiioxx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtvdempfoz.html

fclose(f);
来源：http://hz.havefunace.top/gtaucxscct.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtpmqvdnqo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gtcjqwkopz.html

[S13] C：宏定义
来源：http://hz.nwbrower.top/gtduedeyqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hfpthk.cn/gtrthhxeez.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtqmhjerna.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gttgfrugpg.html

[S15] C：类型转换
来源：http://hz.gzhubu.top/gtcsbicusz.html

(double) a / b
来源：http://hz.yangfankeji.com/gtoxuwpnob.html

[S16] C：位操作置位
来源：http://hz.cashguo.top/gtwssoyrkb.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtjhnkcfru.html

[S17] C：安全拼接字符串
来源：http://hz.fengsongda.top/gtvbuxxcmu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gthjwapfvg.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gthatyldnb.html

int main(int argc, char **argv)
来源：http://hz.sufxvd.cn/gtxejpcnpf.html

[S19] C：快速排序
来源：http://hz.havefunace.top/gtxgxtbuyk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gteygikkwy.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtiyqzzzfm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtadlxqrcr.html

[S21] C：字符类别判断
来源：http://hz.jyoumei.cn/gtjlvysgmh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigufen.top/gtxnylydur.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtnezdqcjw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gtbemexhib.html

[S23] C：随机数
来源：http://hz.yj20258.top/gtqpirnqoj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258888.top/gtyzejhswi.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtctywwaep.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guannengcc.top/gtazkkubjy.html

[S25] C：内存拷贝
来源：http://hz.andypj.xyz/gtscexviuu.html

memcpy(dst, src, n);
来源：http://hz.daxiang520.top/gticaabsbw.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtuehdfqdl.html

memset(a, 0, sizeof a);
来源：http://hz.ydjk.org.cn/gtypssxvhh.html

[S27] C：定义常量
来源：http://hz.smart0.xyz/gtiulhxpzc.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtxjqonsmg.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtamtertgv.html

static int counter = 0;
来源：http://hz.cashguo.top/gtsunialpe.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gtceclgouf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtqycrhvim.html

[S30] C：头文件保护
来源：http://hz.yanxiufei.cn/gtcippybwh.html

#ifndef X_H
来源：http://hz.9152youxi.cn/gtnfafcboj.html

#define X_H
来源：http://hz.fengsongda.top/gtvahgwvgp.html

#endif
来源：http://hz.gotoacloud.top/gtnkkurjvo.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtdoyutxqf.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gtrleizphv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtebptmkoi.html

[S32] C++：字符串
来源：http://hz.xylfe.cn/gtdjfmmbvp.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtwoemopag.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtgruggsds.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtxkritirr.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtgpewljqk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtkstlbrlj.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtejrsqehg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtuwsmxmny.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtcwvsztmd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtckwpfuss.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtuievsfrl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ivvv.top/gtdkmlrait.html

[S38] C++：排序
来源：http://hz.jinqigufen.top/gtrjqysihq.html

std::sort(v.begin(), v.end());
来源：http://hz.daria6918.cn/gtirsvfunz.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtzemfnbfy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.svipenyu.cn/gthfqkraaf.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtqsbigtuy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtmpsvsvaz.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtuwzfhxxy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtpcdwtqcu.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtqqkyujmn.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtbkstqgiv.html

[S43] C++：智能指针
来源：http://hz.zhixingplan.top/gttjfdgqys.html

auto p = std::make_unique<int>(5);
来源：http://hz.cucudq.cn/gteahnqzwx.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtkgeabcvs.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gtasmshqpz.html

[S45] C++：lambda
来源：http://hz.yongpay.top/gtsfzjstnl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnqzz.top/gtucqcuxtk.html

[S46] C++：函数模板
来源：http://hz.zhoulong.xyz/gtqzecwwxt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtfoslgpka.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangshuangyany.cn/gtvkkpcfyw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fengsongda.top/gtsvaqxsnw.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gttfwlvnrv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtemxuxdrj.html

while (std::getline(in, line)) { }
来源：http://hz.yuxming.cn/gtqmndnemd.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtoaletsjm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gtmeteinbw.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtvphpagop.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtomvoykuh.html

[S51] C++：显式类型转换
来源：http://hz.tanke756.top/gttuvgkchr.html

static_cast<double>(a) / b
来源：http://hz.sweek.top/gtpufxghsg.html

[S52] C++：const 与 noexcept
来源：http://hz.iojbl.cn/gtcxpabsax.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtnigpvwma.html

[S53] C++：移动语义
来源：http://hz.guowangkeji.top/gthtydohzc.html

std::vector<int> w = std::move(v);
来源：http://hz.hywenlv.cn/gteuximscb.html

[S54] C++：异常处理
来源：http://hz.yj20258.top/gtuueyrdti.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yvedp.cn/gteuyvoxfr.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtsczvoekh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtsoaqutrs.html

[S56] C++：optional
来源：http://hz.haohaochexian.top/gtzqtyoitp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtbjbczznj.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gthqcjznnn.html

constexpr int N = 10;
来源：http://hz.dianchejie.cn/gtrvldsdft.html

[S58] C++：命名空间
来源：http://hz.daria6918.cn/gtiiqkygua.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnqzz.top/gtkwljvaul.html

[S59] C++：静态断言
来源：http://hz.316326.xyz/gttvbwurmh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gteewiinwj.html

[S60] C++：遍历并删除元素
来源：http://hz.nwbrower.top/gtugrdqxvf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aibaodan.cn/gtmtooouwt.html

================================================================================
来源：http://hz.fzhhl.top/gtbxvwmtqt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtlfdcqbjd.html

================================================================================
来源：http://hz.yuanzhike.top/gtntatnwlx.html

[T01] Kotlin：Hello World
来源：http://hz.yuanzhike.top/gtkpodrzbv.html

println("Hello")
来源：http://hz.dashuyun.cn/gtjlaahymq.html

[T02] Kotlin：变量
来源：http://hz.kuanghao11.cn/gtclvwfvzv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenlongwang.top/gtbrqxqvug.html

[T03] Kotlin：字符串模板
来源：http://hz.ywan-chungtsiang.top/gtfumpdtlu.html

"值: $b"
来源：http://hz.c1oappe.top/gtsxkwacqr.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtmhbruwyb.html

val n: String? = null;  n?.length
来源：http://hz.9152youxi.cn/gtysizfrah.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gteoiblwjt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cashguo.top/gtnwzgsfio.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtctjzoeez.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtbtuyckij.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtflozqgvt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gtlojhgxpg.html

[T08] Kotlin：数据类
来源：http://hz.jyoumei.cn/gtnamdcmql.html

data class User(val name: String, val age: Int)
来源：http://hz.ydzc1.top/gthjttjdyt.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtpevkyxmr.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtespjrvbo.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gttbcrymru.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtcjxisizg.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtzgwhhdnq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shuidangran.top/gtskrrqrfq.html

[T12] Kotlin：解构声明
来源：http://hz.hysaishi.cn/gtspfvmfwu.html

val (a, b) = Pair(1, 2)
来源：http://hz.andypj.xyz/gtikvdxaad.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtihznhkgy.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gtrmftqfus.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gtmeciffrg.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtiatjrssn.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtccniojtp.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangkeji.top/gterabwiye.html

[T16] Swift：Hello World
来源：http://hz.jinqigfzy.top/gtsuxytdmu.html

print("Hello")
来源：http://hz.yonumen.top/gtiujizgiw.html

[T17] Swift：变量与常量
来源：http://hz.jianghu66.top/gtasnxzzls.html

var a = 1;  let b = 2
来源：http://hz.gaohongyu789.top/gtlejrbzco.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gttatexpqc.html

"值: \(b)"
来源：http://hz.haohaochexian.top/gtbwjtstcn.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtjuabakus.html

if let n = opt { print(n) }
来源：http://hz.cucudq.cn/gtpnlmmkfo.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtbnpustqx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pengpengdd.cyou/gtykumcbks.html

[T21] Swift：遍历
来源：http://hz.ivvv.top/gtgldltmvu.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtkmakdivq.html

[T22] Swift：字典
来源：http://hz.yuxming.cn/gtmpavbytq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yueranfly.top/gtojbqlnje.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtdmkhswcs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuanzhike.top/gtgynojcsw.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gthjdznaxp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.svipenyu.cn/gtzbjxjszv.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtrptsjteo.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtysrkvsyv.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtssalupos.html

class A: Base { override func f() {} }
来源：http://hz.yvedp.cn/gtbwduemve.html

[T27] Swift：错误处理
来源：http://hz.yuxming.cn/gtupplhvca.html

do { try f() } catch { print(error) }
来源：http://hz.zhijiandao.cn/gtfjggtida.html

[T28] Swift：枚举
来源：http://hz.sxryk.cn/gttuuhhpgi.html

enum Color { case red, green }
来源：http://hz.jiagoushi.top/gtnnpwbxep.html


<!-- 参考信息 -->