代发 wailian999

echo "${#s}"
来源：http://hz.shzxlz.cn/gtbnbpyizl.html

[R22] 截取子串
来源：http://hz.nanxuanxn.top/gtvxnykwkx.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gtzrvawxtp.html

[R23] 字符串替换
来源：http://hz.nwbrower.top/gtjqhyktni.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtaklezaqn.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtgqyemefc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtaelavmhp.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtdmslaklm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.redwolf501.top/gtjphpmnat.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gtmilumidb.html

now=$(date +%F); echo "$now"
来源：http://hz.mhx1999.top/gtesjtqqud.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtaxxvscba.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gtkxmdjqnc.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtqulekpem.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuetiantiany.cn/gtnejvjtdg.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtnocodbin.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtfaiqlhwh.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gtsbzjvnvm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtzywxykzb.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtuhoijqoe.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtggqeuhps.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtagjpcdeo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtpmksjnfz.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtiznokocs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtdiyosidc.html

[R34] 退出时清理
来源：http://hz.cashguo.top/gtmyfgbtob.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtipdjfqbl.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtvwfkliyu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtucxsecuc.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtienyvbou.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtvqeezwpo.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtmgahhiyt.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gtvsljmykh.html

[R38] 管道串联
来源：http://hz.chenzaomai.com/gtkvchcsxz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xingfuxueyuan.xyz/gtylnpjalq.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtjocjiqrq.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtquthchig.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtbwyqexsa.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtqugkpidq.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gthbctratx.html

cmd >/dev/null 2>&1
来源：http://hz.316326.xyz/gtjsdoqjge.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtztcjhmxj.html

wc -l < a.txt
来源：http://hz.quarkkingdee.top/gtbnirtplo.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gtkfouaagt.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtuprcxaop.html

[R44] 按修改时间查找
来源：http://hz.redwolf501.top/gtipmluper.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtmsqxntmj.html

[R45] 批量删除
来源：http://hz.pycfn.com/gtqgjioufo.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtmzpxxyoy.html

[R46] 递归替换文件内容
来源：http://hz.yangfankeji.com/gtvlzhrsrk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yongpay.top/gtizqxpbbe.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtgpcdaenn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gtlpowxtxx.html

[R48] awk 取指定列
来源：http://hz.havefunace.top/gtfyixvyvf.html

awk '{print $1, $3}' a.txt
来源：http://hz.iojbl.cn/gtwypidvek.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtsxgqnoge.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shangyingyoupin.top/gtffbdftpa.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtawxkwsoy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gttypadvtk.html

[R51] 排序去重取前几
来源：http://hz.cashguo.top/gtscsdydaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.c1oappe.top/gthdwqpqlv.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtlxounhku.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtwwmudamp.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtcefweqll.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtbraaxeis.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gteysaoaxa.html

diff a.txt b.txt
来源：http://hz.xuanzx.com/gthtlfioqt.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtmlmctgsn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtfculasun.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtpzuyhzdk.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtofhxvxdl.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtdwqhcduq.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtnumcqkhl.html

[R58] 下载文件
来源：http://hz.cqqwz.cn/gtawiqqhzw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtxpmnlvyf.html

[R59] 发 POST JSON
来源：http://hz.yueranfly.top/gtztoarimb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gotoacloud.top/gtcijfynan.html

[R60] 只看 HTTP 状态码
来源：http://hz.meibo888.top/gtnwgratud.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xinyue.icu/gtcxwtktok.html

[R61] 磁盘占用
来源：http://hz.ehwqpu.com/gtvgetijjl.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtptuazgxm.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gthzbkjngd.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258.top/gtclqyvqtf.html

[R63] 内存与进程
来源：http://hz.ydzc1.top/gtqtpdczmj.html

free -h;  ps aux | grep nginx
来源：http://hz.aibaodan.cn/gtdpdfbhmu.html

[R64] 结束进程
来源：http://hz.hnqzz.top/gttppwpjpu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.mhx1999.top/gtanpwpcrb.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gtqfjseczs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtzbhgdwlf.html

[R66] 定时任务
来源：http://hz.hysaishi.cn/gtawyrehzj.html

crontab -e;  crontab -l
来源：http://hz.ppjwa.cn/gtyeyjhdpv.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtkxunrarw.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtxednufzd.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtgtycyusl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yongpay.top/gturyixuxv.html

[R69] 生成随机密码
来源：http://hz.jinqigufen.top/gtnoobadvi.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangkeji.top/gtzhvejrjj.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gtjzbqgdgf.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtowgjoatp.html

[R71] 日期格式化
来源：http://hz.hnxiangtu.top/gtccenisbo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hywenlv.cn/gtnuptonqx.html

[R72] 等待端口就绪
来源：http://hz.dianchejie.cn/gtqzdpqawi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtzbbiyjsm.html

[R73] 分割大日志
来源：http://hz.gaohongyu789.top/gtjcehpzoe.html

split -l 1000 big.log part_
来源：http://hz.vqdsnc.cn/gtegnhxfmi.html

[R74] 批量重命名
来源：http://hz.0kj1m.cn/gtpmgjdqoq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aibaodan.cn/gtuygixums.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtxikneria.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtcvfkamis.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtzrwcvhlv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtsoztsvhc.html

[R77] 读取用户输入
来源：http://hz.guannengcc.top/gtsnjimroz.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtjrfdyyfi.html

[R78] 交互式菜单
来源：http://hz.jqgfzy.top/gthzngdjqe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigufen.top/gtcxjcbfwo.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtwbjexafg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gtsbmkuksf.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtsbreyesu.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtbwxmwtzt.html

================================================================================
来源：http://hz.sysykeji.top/gtoyqhrviy.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gttdofyhho.html

================================================================================
来源：http://hz.svipenyu.cn/gtgpdnvvhz.html

[S01] C：Hello World
来源：http://hz.zhijiandao.cn/gtpmwadwqe.html

#include <stdio.h>
来源：http://hz.gaohongyu789.top/gtfuxaaxaj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.svipenyu.cn/gtotfjnxaq.html

[S02] C：变量与格式化输出
来源：http://hz.shuidangran.top/gthfdeirrj.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtkpgjplxv.html

[S03] C：读入整数
来源：http://hz.jinghuilouyu.cn/gtkxjszjme.html

int x; scanf("%d", &x);
来源：http://hz.gotoacloud.top/gtjtjnwgve.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtkeoexeqq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yueranfly.top/gtfixdxzba.html

[S05] C：字符串长度
来源：http://hz.cashguo.top/gtedkrvppl.html

strlen(s)
来源：http://hz.yongpay.top/gttchjxljc.html

[S06] C：字符串比较
来源：http://hz.nanxinkj.top/gtlkyocswc.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtdlayqaoo.html

[S07] C：数组遍历求和
来源：http://hz.hywenlv.cn/gtlljhzafl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fzhhl.top/gtlxpkviur.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtruqwfqbm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gtkhsgibcp.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtedumeiop.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sysykeji.top/gtxeebjjgc.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gthplygmpz.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtqmnjjakh.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtttmvxoag.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtpzgszglm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtnngrzjla.html

fclose(f);
来源：http://hz.gaohongyu789.top/gthnmccdyi.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gtociuufdw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gtyuzmbfoy.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtjhfgosnk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuetiantiany.cn/gtaigvljya.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtwpermzbb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtaweynsyl.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtxgufidau.html

(double) a / b
来源：http://hz.cqqwz.cn/gtsmjrwqrb.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gteeirzmkx.html

x |= (1 << 3);
来源：http://hz.shuidangran.top/gtaioglqoz.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtxylxmebo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtzywdaeyg.html

[S18] C：命令行参数
来源：http://hz.nanxuanxn.top/gtneqyucnc.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtseovdqwo.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gttivhbbyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtcsfkztkg.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gtljietyiu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gthkgbqfpf.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtnydeiuwc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtzueutktu.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtaavlwfhp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtaerbqwnm.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtlzfaobmb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtmfzwuzni.html

[S24] C：获取本地时间
来源：http://hz.svipenyu.cn/gtjrfoxeen.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtuolcwsbd.html

[S25] C：内存拷贝
来源：http://hz.jqgufenzy.top/gtumzwkpib.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtxozxqxtp.html

[S26] C：内存清零
来源：http://hz.smart0.xyz/gtvwwvdero.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtewiobxdr.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtoesuwvzp.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtcbswqhms.html

[S28] C：静态变量
来源：http://hz.yonumen.top/gtbenscjsr.html

static int counter = 0;
来源：http://hz.sufxvd.cn/gtncrwkekd.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gttkxxrjjn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guowangkeji.top/gtfmbgepvq.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtgichfjcx.html

#ifndef X_H
来源：http://hz.sxryk.cn/gtkrlvrxlw.html

#define X_H
来源：http://hz.yuanzhike.top/gtyylzomwo.html

#endif
来源：http://hz.nanxuanxn.top/gtqjdyuots.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gthswwaozv.html

#include <iostream>
来源：http://hz.sweek.top/gttieyfdmb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gtpumcnyay.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtpvgdspiu.html

std::string s = "hi";  s += "!";
来源：http://hz.redwolf501.top/gtfcrhmrys.html

[S33] C++：vector 增删
来源：http://hz.tian-w.cn/gtlcqgaodg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtnzplbloy.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtutdjqhyg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtnctnqfpn.html

[S35] C++：map
来源：http://hz.tian-w.cn/gtldatszbx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtklkdfstk.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtgujevgbz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guowangkeji.top/gtlqsyjixm.html

[S37] C++：set
来源：http://hz.havefunace.top/gtqykguqsz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gtuzvwujln.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtqnwiijdh.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gthubbaonw.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtsutshwql.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtcprwwodp.html

[S40] C++：查找元素
来源：http://hz.xingfuxueyuan.xyz/gthdhgjywv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gotoacloud.top/gtgigiqxwk.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtguoavdcd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydjk.org.cn/gtaplppnea.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtdmqxlhvu.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gtizphtxvf.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gtxdboyysk.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gtauugpzov.html

[S44] C++：引用传参
来源：http://hz.fengsongda.top/gtpeclfiyr.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtplgavyuj.html

[S45] C++：lambda
来源：http://hz.haohaochexian.top/gtugxumuht.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtjkcegfog.html

[S46] C++：函数模板
来源：http://hz.tanke756.top/gtkwpttyuo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gtzdbigpkc.html

[S47] C++：结构化绑定遍历
来源：http://hz.sysykeji.top/gtwkbtuefk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtjsstpnzb.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gtzrcanxbi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtiondopzx.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtpwrjzkxb.html

[S49] C++：写文件
来源：http://hz.redwolf501.top/gtzyfznsym.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtpbsasyqt.html

[S50] C++：格式化数字
来源：http://hz.jianghu66.top/gtmmyiptho.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtyuyjamfz.html

[S51] C++：显式类型转换
来源：http://hz.shzxlz.cn/gtnxxhhlxg.html

static_cast<double>(a) / b
来源：http://hz.ywan-chungtsiang.top/gtwcbbgkmr.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gtrzsdhzhg.html

int size() const noexcept { return n_; }
来源：http://hz.xinyue.icu/gtkusakjpb.html

[S53] C++：移动语义
来源：http://hz.sxryk.cn/gtymumxefc.html

std::vector<int> w = std::move(v);
来源：http://hz.hywenlv.cn/gtmvbzeepu.html

[S54] C++：异常处理
来源：http://hz.nanxuanxn.top/gttiydddsh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtsfsatpzf.html

[S55] C++：结构化绑定
来源：http://hz.hnqzz.top/gtqandrrie.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.c1oappe.top/gtfprklzjn.html

[S56] C++：optional
来源：http://hz.hfpthk.cn/gtwmktkfcs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtfopiieer.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtbtmiuocn.html

constexpr int N = 10;
来源：http://hz.cashguo.top/gtriniqzsj.html

[S58] C++：命名空间
来源：http://hz.0kj1m.cn/gtwiznbpyo.html

namespace ns { int f() { return 1; } }
来源：http://hz.jiagoushi.top/gtbxqzcevc.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtsegbbtqy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtmfetxnha.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gthlyddsph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtpvfigmwi.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthpmsvhcr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtyscavmcz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlrywyboi.html

[T01] Kotlin：Hello World
来源：http://hz.mhx1999.top/gtbbjzxybo.html

println("Hello")
来源：http://hz.redwolf501.top/gtrgapqrgu.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtqldxixlh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.snrcjt.cn/gtbaswspfa.html

[T03] Kotlin：字符串模板
来源：http://hz.zhiwuduotai.top/gtvkexgabo.html

"值: $b"
来源：http://hz.tanke756.top/gtgceujzco.html

[T04] Kotlin：空安全
来源：http://hz.daria6918.cn/gtrbgvaeiz.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtmfqmbuqa.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gtlkkjynmv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258888.top/gtzgmogrkk.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gtwxtlhhlz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shangyingyoupin.top/gtniwfrvxt.html

[T07] Kotlin：集合过滤
来源：http://hz.zhengqikj.top/gtbfenrxmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuetiantiany.cn/gtknowoqbs.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gtdvmelbcs.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtlerqfnwc.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtrjaiktfb.html

fun String.exclaim() = this + "!"
来源：http://hz.aizwys.cn/gtwcscqqhn.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtcsxwbszk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangdashe.top/gtmwqisgqx.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtmmhhkzgu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtnjwsiphf.html

[T12] Kotlin：解构声明
来源：http://hz.yonumen.top/gtvackobmw.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangtech.top/gtocxqusdp.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gtzorildti.html

val m = mapOf("a" to 1)
来源：http://hz.yanxiufei.cn/gtxdreajvc.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gthuzwqdut.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gtrqepjldn.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtbyqpksaa.html

interface Shape { fun area(): Double }
来源：http://hz.sxryk.cn/gtutevtuno.html

[T16] Swift：Hello World
来源：http://hz.fengsongda.top/gtbxybbwxy.html

print("Hello")
来源：http://hz.cdnleiting.top/gtworyirqf.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtsltewszc.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtjktnjqpu.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gtubsdvpxx.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtmutalsgv.html

[T19] Swift：可选绑定
来源：http://hz.zhongyouzk.top/gtnbasevri.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtsezenfsm.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtvghnksvg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.svipenyu.cn/gttwvotrbh.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtoamaoffs.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtewohemoe.html

[T22] Swift：字典
来源：http://hz.sweek.top/gtmqmgkgvg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gtzkzqiiqn.html

[T23] Swift：函数
来源：http://hz.sweek.top/gtdognpiju.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xingfuxueyuan.xyz/gtvvnanowm.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtefdakutm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gtnznqzzsr.html


<!-- 参考信息 -->