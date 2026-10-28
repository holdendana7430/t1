代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtsaavsfkf.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtzrgdmpcs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.52xcode.cn/gttljstaey.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtjjpfywfx.html

f() { local x=1; echo "$x"; }
来源：http://hz.bjfxy.top/gtywcdnhlf.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtzmkwgyin.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtxpinbeax.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtoqlumper.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtletofuve.html

[R34] 退出时清理
来源：http://hz.jyoumei.cn/gtzfjtelyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtveyccrjb.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtuwugmidf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gttmdqidgb.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtyhgurwrq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhengqikj.top/gtmqnpsmpi.html

[R37] 把输出赋给变量
来源：http://hz.fengsongda.top/gtfnnmigrc.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtrewaiusu.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtdjrgfrjd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtmguvgmpb.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtpdfkfhld.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtsonpdwgp.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gthgdxjvja.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtsnmreqgz.html

[R41] 丢弃输出
来源：http://hz.jyoumei.cn/gteibbudpi.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtbysqmmwf.html

[R42] 输入重定向
来源：http://hz.gaohongyu789.top/gtkceyeftf.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtofrhjslk.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtcdxuyscs.html

find . -name "*.log" -type f
来源：http://hz.yueranfly.top/gtylafvodw.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtlajjemdo.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtbgnsutvb.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtdflqrmbt.html

find . -name "*.tmp" -delete
来源：http://hz.ehwqpu.com/gtyaabmrxq.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtjmmvbdrm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtxlyzqylm.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtpqhwpxgn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtmameybrx.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gtjuohvwij.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtmywjhige.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtgpjybpuc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hongshengwenyu.top/gtwizofycl.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtwyoftppl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtrzocsqbj.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtzkcisrsh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtlqkkslcy.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtalusnqpe.html

wc -l a.txt
来源：http://hz.nanxuanxn.top/gtgvmvyfbd.html

[R53] 查看文件头与实时尾
来源：http://hz.ehwqpu.com/gtaubabrfo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtrevbwass.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gtgpdxknht.html

diff a.txt b.txt
来源：http://hz.52xcode.cn/gttuwdeztb.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gtrhisdnzu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shangyingyoupin.top/gtizzkdyyx.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtnzmvylev.html

scp file user@host:/path/
来源：http://hz.tanke756.top/gtjekbduul.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtraibqpnc.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtxrpvvwjd.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtyicwlgpk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtdokvusmx.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtfcjaihak.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gthalxdtbn.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtkxwcxynd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhongyouzk.top/gtdbnoizwg.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtydzzhubt.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtitiivhrz.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtfirotzcu.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258888.top/gtmfcdicnk.html

[R63] 内存与进程
来源：http://hz.hnxiangtu.top/gtgpqzxfke.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtfyylgotf.html

[R64] 结束进程
来源：http://hz.yj202588.top/gttkekelbj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtccvcdfui.html

[R65] 查看端口占用
来源：http://hz.gaohongyu789.top/gtdiekfcoc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.haohaochexian.top/gtevbevelk.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtalcstmlu.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtwaqhwgeu.html

[R67] 生成随机十六进制串
来源：http://hz.ivvv.top/gtvxsjuire.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtlpavhgdi.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gtutlgfqqo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtysikhgdn.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtavrjidah.html

head -c 16 /dev/urandom | base64
来源：http://hz.iojbl.cn/gtphxfsnca.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtxvnouquf.html

date +%s;  date -d @1700000000
来源：http://hz.jianghu66.top/gtgqrnymrt.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtzoxuefyu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtidhctzwr.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtvrfdrtex.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtepsiqerv.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gtxfxxsdou.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtpcbbtnmk.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtkzhbtnvv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtlynicyzu.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtarejkskf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gtmyicbmoz.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtcnijpduv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtsjjlcxnl.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtiuzxemvo.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtlikzcfrq.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtojahjyll.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtarpjldnh.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangtech.top/gtwspvismj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.svipenyu.cn/gtspkjijoh.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gtzhjjurlw.html

time ./run.sh
来源：http://hz.birdmap.top/gtagcbymhs.html

================================================================================
来源：http://hz.iojbl.cn/gtntjydixc.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtlyjyqrmn.html

================================================================================
来源：http://hz.snrcjt.cn/gtviqmofgd.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtiymmbswy.html

#include <stdio.h>
来源：http://hz.cucudq.cn/gtcarktljx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgufenzy.top/gtuznhwuzv.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258888.top/gtvvmqebem.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtjuwmrvsu.html

[S03] C：读入整数
来源：http://hz.jinyuanbaomall.cn/gtjknohhip.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtytdendsr.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gtphtlrlik.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtoqqfqfak.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtgahsidjo.html

strlen(s)
来源：http://hz.jiagoushi.top/gtfmdmqoge.html

[S06] C：字符串比较
来源：http://hz.yvedp.cn/gtljrsvpfv.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtfqyysplq.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtymksnevq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtoqqumujj.html

[S08] C：动态内存分配与释放
来源：http://hz.pengpengdd.cyou/gtwrwpcgjl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtozgnhufs.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtltqjrvxv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtsfqpeefi.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtkpxfmzwz.html

int *p = &a;  *p = 5;
来源：http://hz.zhaomingkeji.xyz/gtchylzfam.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtvwmbmsrt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtcffedldc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtpndqgwwa.html

fclose(f);
来源：http://hz.redwolf501.top/gtyfdoloaa.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtvrabnwox.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sufxvd.cn/gtweyzclud.html

[S13] C：宏定义
来源：http://hz.dashuyun.cn/gtptkqhjxz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jianghu66.top/gtotmhwwlm.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtdjdcmzeq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtqhvhythf.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtjrorbfxu.html

(double) a / b
来源：http://hz.wangdashe.top/gtmshucmxb.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtbfaigjdk.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gtimupiehb.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtkxutxcxs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pycfn.com/gtvphfkoia.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtdsbyquik.html

int main(int argc, char **argv)
来源：http://hz.aibaodan.cn/gthssodkyb.html

[S19] C：快速排序
来源：http://hz.sufxvd.cn/gtihicbgna.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtfytvoiop.html

[S20] C：二分查找
来源：http://hz.havefunace.top/gtcjoaauzq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtvolwyudp.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtjhzqdzua.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtjlxcgsue.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtkzvdekrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yanxiufei.cn/gttjlcednq.html

[S23] C：随机数
来源：http://hz.cashguo.top/gtvspvpvdb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtvruahjwy.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gtibodqrsd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sufxvd.cn/gtckbfpffx.html

[S25] C：内存拷贝
来源：http://hz.hammf.cn/gtjqnpcdas.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtbkuajnbj.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtnamaajwc.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtbmgbcgko.html

[S27] C：定义常量
来源：http://hz.havefunace.top/gtwjxcsllb.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtzwtuzdye.html

[S28] C：静态变量
来源：http://hz.gotoacloud.top/gtmqydgwnd.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtgdbwgiql.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gtaxjroxrj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtwrgnpbxq.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtophetpum.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtzjaxldnj.html

#define X_H
来源：http://hz.yonumen.top/gtpadckkrv.html

#endif
来源：http://hz.iojbl.cn/gtzzshvsvq.html

[S31] C++：Hello World
来源：http://hz.sufxvd.cn/gtqvaacnjm.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gtftnhuojg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.redwolf501.top/gtxjkogoks.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtwelztqaj.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gtekhwwerh.html

[S33] C++：vector 增删
来源：http://hz.sxryk.cn/gtvsebtpqd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhongyouzk.top/gtfsljztnp.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtldfysvkr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtedlxomdi.html

[S35] C++：map
来源：http://hz.zdqjudy.top/gtqiflhldy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtvbynvlkt.html

[S36] C++：unordered_map
来源：http://hz.hongshengwenyu.top/gtsjnyqzbe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtjxxqnegh.html

[S37] C++：set
来源：http://hz.yuxming.cn/gtzbrhgdpf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nwbrower.top/gtawvnnopx.html

[S38] C++：排序
来源：http://hz.0kj1m.cn/gtrsckfhzo.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtcbrorysn.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtvjxkeojd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtoctecwqd.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtltrrkuym.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tian-w.cn/gtomifsjqy.html

[S41] C++：类与构造函数
来源：http://hz.shuidangran.top/gtdrslasbt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xylfe.cn/gtsfqtidaw.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtfgohzkgm.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gtspolkxfv.html

[S43] C++：智能指针
来源：http://hz.iojbl.cn/gtonlynnit.html

auto p = std::make_unique<int>(5);
来源：http://hz.bjfxy.top/gtxxgmitjj.html

[S44] C++：引用传参
来源：http://hz.hnqzz.top/gtecsomstm.html

void inc(int &x) { ++x; }
来源：http://hz.daria6918.cn/gtutoqvpcw.html

[S45] C++：lambda
来源：http://hz.fzhhl.top/gtqdzfvtpz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gttpjcldxj.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtgokxlshy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gtfwnwhcds.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenzaomai.com/gtsodqksun.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gtwesryaxj.html

[S48] C++：逐行读文件
来源：http://hz.zycfv.cn/gtvzzdqjid.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cheryme.top/gtujpkplkx.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtiokkphyu.html

[S49] C++：写文件
来源：http://hz.ehwqpu.com/gtpzrzkkva.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtdwlnlzzb.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtxctxxcnp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gogol.net.cn/gtqmibrktz.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtlmmkaiwh.html

static_cast<double>(a) / b
来源：http://hz.dianchejie.cn/gtwgxmzivm.html

[S52] C++：const 与 noexcept
来源：http://hz.dashuyun.cn/gtemxrljmr.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtnbrxbyid.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangtech.top/gthaxfadiw.html

std::vector<int> w = std::move(v);
来源：http://hz.jinyuanbaomall.cn/gtrmsapsdd.html

[S54] C++：异常处理
来源：http://hz.dashuyun.cn/gtdbtdakxa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gthegdaxas.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtbxaxaayt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pengpengdd.cyou/gttqomyqwq.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtkbjdmxak.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gtisjldwro.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtjqyzwnsh.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtktnzoaxp.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtikwsiupc.html

namespace ns { int f() { return 1; } }
来源：http://hz.fengsongda.top/gtvrdnlayc.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtovgwmufv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258.top/gtwrqjopef.html

[S60] C++：遍历并删除元素
来源：http://hz.yuxming.cn/gthakcutca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhoulong.xyz/gtfloilyjm.html

================================================================================
来源：http://hz.cucudq.cn/gtdqjsxgee.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gtimlgmwbh.html

================================================================================
来源：http://hz.guowangkeji.top/gtbigqqtqc.html

[T01] Kotlin：Hello World
来源：http://hz.xuetiantiany.cn/gtiembslpb.html

println("Hello")
来源：http://hz.cheryme.top/gtdwkdnsil.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtkvucmerv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtuvrqabny.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gthxmgnmhk.html

"值: $b"
来源：http://hz.xylfe.cn/gtchrfzqme.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gttnawyfso.html

val n: String? = null;  n?.length
来源：http://hz.gotoacloud.top/gtjvlsogub.html

[T05] Kotlin：when 表达式
来源：http://hz.yanxiufei.cn/gtlbdpfguj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258888.top/gtysnjqbbz.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtntbbbdai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtbicflrpn.html

[T07] Kotlin：集合过滤
来源：http://hz.chenzaomai.com/gtmwpuiowz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zycfv.cn/gtqjbpqfnm.html

[T08] Kotlin：数据类
来源：http://hz.cucudq.cn/gtqbsvyzda.html

data class User(val name: String, val age: Int)
来源：http://hz.bjfxy.top/gtjczeibqu.html

[T09] Kotlin：扩展函数
来源：http://hz.fengsongda.top/gtuhjvvakg.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtynaksmkg.html

[T10] Kotlin：默认参数
来源：http://hz.shzxlz.cn/gthzmvxhpu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhijiandao.cn/gtbqfrdozx.html

[T11] Kotlin：协程
来源：http://hz.cashguo.top/gtmidizhwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.iojbl.cn/gtxlfhcpvq.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtfnymoywf.html

val (a, b) = Pair(1, 2)
来源：http://hz.yonumen.top/gtzdwnxbql.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtpffjytot.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtjnndhaau.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtyfdhcfmu.html

for (i in 1..10) println(i)
来源：http://hz.jinqigfzy.top/gtdxnhtlgz.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtaxbyvmmg.html

interface Shape { fun area(): Double }
来源：http://hz.smart0.xyz/gtaetcskkc.html

[T16] Swift：Hello World
来源：http://hz.tianlin.xyz/gtkftiwpav.html

print("Hello")
来源：http://hz.yj202588.top/gtvnpfbbwz.html

[T17] Swift：变量与常量
来源：http://hz.ydjk.org.cn/gtmvtckybk.html

var a = 1;  let b = 2
来源：http://hz.nwbrower.top/gtplhvdzzj.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtmbeduant.html

"值: \(b)"
来源：http://hz.nwbrower.top/gtmwtmfwej.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gtwwakurte.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtcazfxlka.html

[T20] Swift：数组操作
来源：http://hz.cashguo.top/gtlfiukfwt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtitzmuevh.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gtngljculk.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtwmbbkiml.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gtblciroqp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xziqi.cn/gtnxobafzz.html

[T23] Swift：函数
来源：http://hz.fzhhl.top/gtyuftizox.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gtxkzfilhu.html

[T24] Swift：闭包
来源：http://hz.jqgufenzy.top/gtrajwqgmh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtvwefyfeo.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtmqaletns.html

struct P { var x: Int }
来源：http://hz.chenzaomai.com/gtgwkasorp.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gtqrioyvol.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtsqqerhcf.html

[T27] Swift：错误处理
来源：http://hz.hfpthk.cn/gtohuadxvu.html

do { try f() } catch { print(error) }
来源：http://hz.redwolf501.top/gtcfxolmmu.html

[T28] Swift：枚举
来源：http://hz.jianghu66.top/gtmrijcikp.html

enum Color { case red, green }
来源：http://hz.zdqjudy.top/gtnymksuqe.html

[T29] Swift：guard 提前返回
来源：http://hz.cheryme.top/gtmfaabutu.html

guard let x = opt else { return }
来源：http://hz.chenjidiqi.icu/gtborqwhtp.html

[T30] Swift：协议
来源：http://hz.52xcode.cn/gthcykzmfy.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtmzkbzkpc.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtuivufqgm.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtdqppqtkl.html

[T32] Lua：局部变量
来源：http://hz.yonumen.top/gtveafwxbi.html

local a = 1
来源：http://hz.fengsongda.top/gtmpqlahlj.html


<!-- 参考信息 -->