代发 wailian999

echo "${#s}"
来源：http://hz.aizwys.cn/gtqegihccq.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gtrvbneadc.html

echo "${s:0:5}"
来源：http://hz.zdqjudy.top/gtltjzlwgh.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtqhqxewui.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtyqpmrzmw.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtaebtojnm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtgqloieax.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtopxstflo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtxsboagtg.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtpaqedppl.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtybhlhnhf.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtthzugkdt.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtzdewgunq.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtctmdotwr.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtrmrnthrq.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtentmfcdz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtjhtvbmzh.html

[R30] 函数返回状态码
来源：http://hz.316326.xyz/gtbnpnmfzz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.c1oappe.top/gtxfkeszqf.html

[R31] 局部变量
来源：http://hz.tanke756.top/gtetbkuagd.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtrsxzhfwy.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtswoobqny.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dianchejie.cn/gtwpjhwosl.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtdggfqffj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtutjwdwam.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtjqytjrym.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gthpbrljjn.html

[R35] 后台执行并等待
来源：http://hz.wangdashe.top/gtvpxbxrlx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.9152youxi.cn/gtezgthnow.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtsdkzzxwl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangshuangyany.cn/gtbnopdocv.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gtfepyttnz.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtbpntfdvc.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtvuijwsyx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtwpwscafj.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gtavhzwemq.html

cmd > out.log 2>&1
来源：http://hz.nanxinkj.top/gtwjcnhqdk.html

[R40] 追加写日志
来源：http://hz.hnxiangtu.top/gttyoqzrsz.html

echo "log" >> out.log
来源：http://hz.hywenlv.cn/gtfktktswe.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtmuuewlhs.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtmdvxzbli.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtuualbblk.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtxkylanza.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtnnwfzosf.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtvdbschjm.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtxkxjawus.html

find . -mtime -7 -type f
来源：http://hz.jinqigufen.top/gtibxncmfz.html

[R45] 批量删除
来源：http://hz.sufxvd.cn/gtkncgqzyy.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtwcctdaos.html

[R46] 递归替换文件内容
来源：http://hz.52xcode.cn/gtswlyfhhu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtobshebca.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtpzzeslwy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ehwqpu.com/gtwczfwgln.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtkndbbsti.html

awk '{print $1, $3}' a.txt
来源：http://hz.hongshengwenyu.top/gtttqsdcrt.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtqbzqqehe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtthqpjprs.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gttddjovgg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gthpvfcval.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtkxpgxhcu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fengsongda.top/gteuuxqxbu.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gtntsemnda.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gtorxmnahf.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtivmfzzhj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtecxjhvqs.html

[R54] 比较两个文件
来源：http://hz.feifeiyinyue.top/gtqjhjuqak.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtshhihsrk.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtcizvxcxc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jianghu66.top/gttrzgmlvo.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gttzhcjrum.html

scp file user@host:/path/
来源：http://hz.fzhhl.top/gtrkdrgnct.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtcyiwsqrh.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtjebuvxji.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtisjmlsry.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gttgmtndbr.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtnayiqcbi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtjoiwldmj.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtrffdrubw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pycfn.com/gttccnomxw.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gthfdcevee.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtmebsnjrk.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtrsugpygj.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gttioelxmx.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtnrypafsf.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtrnvsjvls.html

[R64] 结束进程
来源：http://hz.tanke756.top/gtucymtuyy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtgaqerjxy.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtxaewgnmd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gtqympcqlq.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gtwkqshsxm.html

crontab -e;  crontab -l
来源：http://hz.yonumen.top/gtddtadday.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gticimdnow.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gtmwbbjxua.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtxhpfxqlo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtbvofztnd.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtzufmbxyd.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtrodpmuxe.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtdowpjkky.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtdqeuitbs.html

[R71] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtyhpuixln.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtfajupbva.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gthgcwdgpk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtdzlewslj.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gtngtedjtf.html

split -l 1000 big.log part_
来源：http://hz.haohaochexian.top/gticszufdf.html

[R74] 批量重命名
来源：http://hz.tanke756.top/gtepibdmbj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pengpengdd.cyou/gtmngicpcj.html

[R75] 导出环境变量
来源：http://hz.zhaomingkeji.xyz/gtrkkivlgi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gtiywzodzc.html

[R76] 使用临时文件
来源：http://hz.xylfe.cn/gtmrixavhq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtigswacqa.html

[R77] 读取用户输入
来源：http://hz.shzxlz.cn/gtppxrlxfv.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtpxpuruoj.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtgbkcfxrf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gtutitbyql.html

[R79] 解析命令行选项
来源：http://hz.daria6918.cn/gtldcchzce.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ivvv.top/gtrqlwislg.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtmwdyufcu.html

time ./run.sh
来源：http://hz.cucudq.cn/gtkhjvakpm.html

================================================================================
来源：http://hz.hammf.cn/gtyaqrgulx.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtufqycdab.html

================================================================================
来源：http://hz.guowangkeji.top/gtzcteogxf.html

[S01] C：Hello World
来源：http://hz.cqqwz.cn/gtcomkvgbn.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtahdxqyrt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gtsrimrdfy.html

[S02] C：变量与格式化输出
来源：http://hz.hammf.cn/gtnftspkhl.html

int a = 10; printf("%d\n", a);
来源：http://hz.fzhhl.top/gtxdjdhxxc.html

[S03] C：读入整数
来源：http://hz.yvedp.cn/gtlhonwfgo.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtwpopygha.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtkpttkfqs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangtech.top/gttvufimkk.html

[S05] C：字符串长度
来源：http://hz.nanxinkj.top/gtiroawmeg.html

strlen(s)
来源：http://hz.redwolf501.top/gtehcwglks.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtvesoozlw.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtbwnckrum.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtklgfxlqy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ehwqpu.com/gtfceqiluc.html

[S08] C：动态内存分配与释放
来源：http://hz.zhijiandao.cn/gtvwjptquu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gtvjvutkli.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtjvnpmtwo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.redwolf501.top/gtwnmgpvyt.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtyifmbpsm.html

int *p = &a;  *p = 5;
来源：http://hz.gogol.net.cn/gtfuerpskx.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtbfnqanyh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxinkj.top/gtvqhfktfd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gthypufmfl.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtmmjmzuzv.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtzouhuqec.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtafcuxzbq.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtsmyajhnk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtulpwrpmj.html

[S14] C：枚举
来源：http://hz.hammf.cn/gtokolgbjd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shuidangran.top/gtbcqsihna.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtdsqyrata.html

(double) a / b
来源：http://hz.sufxvd.cn/gtptqxtvfi.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtfuxuzzfd.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtziltbtrp.html

[S17] C：安全拼接字符串
来源：http://hz.jinghuilouyu.cn/gtfilwtguh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gttvrlelku.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtjbomuirs.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtzjrbutly.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtjcbdaxhb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtlvzzhduy.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtwjwaffbv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtxkveidne.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtveweuefr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtjsmizxhl.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtjveaicfv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.quarkkingdee.top/gtjhyrhtow.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtfbiivawl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtfjldeyet.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gthgtcrzby.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tanke756.top/gtpjqjwyww.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtwtaqyiyq.html

memcpy(dst, src, n);
来源：http://hz.gzhubu.top/gtywgnrbjv.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtnkzfvkal.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtkriscfom.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtpdsdvaxz.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtarkbrkps.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtvzzmavou.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtvtpbfgqz.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtqevrhgmj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtajowhckw.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gttppcwswx.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtzwmngfmy.html

#define X_H
来源：http://hz.smart0.xyz/gtbgxhbrku.html

#endif
来源：http://hz.ivvv.top/gtypwociyy.html

[S31] C++：Hello World
来源：http://hz.redwolf501.top/gtvtkpshae.html

#include <iostream>
来源：http://hz.shanyushiyangkeji.top/gtpiiibomk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtlhomkcmr.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gtikudatxy.html

std::string s = "hi";  s += "!";
来源：http://hz.zdqjudy.top/gtojmxeszp.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtjlxtorwx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtrtsexyvz.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtovufrwhl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.havefunace.top/gtthfjywsk.html

[S35] C++：map
来源：http://hz.chenzaomai.com/gtdmttphsb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gthztvcjln.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtljbgslbe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtbezrkitg.html

[S37] C++：set
来源：http://hz.smart0.xyz/gtkjkqxwzl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtrtvbpbkh.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtsxdlntnd.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtkffivxuc.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gtjlnjapib.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtpmmfeenl.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtgwjknidr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtrjneddzj.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtunkgblwk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtxivcgsyk.html

[S42] C++：继承与虚函数
来源：http://hz.jqgfzy.top/gtmxmrxemc.html

class B : public Base { public: void f() override {} };
来源：http://hz.dianchejie.cn/gthmxzqakz.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtpzkrjent.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gttjygeaod.html

[S44] C++：引用传参
来源：http://hz.quarkkingdee.top/gthfwkbaui.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gtskbdvzfi.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtqcyhfcbb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtidssmotq.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtrnjstawj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinghuilouyu.cn/gtvikrzios.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258.top/gtorvlailx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.redwolf501.top/gtshqrkrkf.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gttfjlmaug.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtuzrsrxsa.html

while (std::getline(in, line)) { }
来源：http://hz.xylfe.cn/gtcjkkfmiv.html

[S49] C++：写文件
来源：http://hz.yanxiufei.cn/gtyuriijrh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ivvv.top/gtbzvpqtkn.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtfsvvlcmc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtbgvdlmao.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtxqbevwia.html

static_cast<double>(a) / b
来源：http://hz.nanxinkj.top/gtrhvkalai.html

[S52] C++：const 与 noexcept
来源：http://hz.fzhhl.top/gtdkgabwmb.html

int size() const noexcept { return n_; }
来源：http://hz.xuetiantiany.cn/gtkzhepgpq.html

[S53] C++：移动语义
来源：http://hz.pengpengdd.cyou/gttzpbuojf.html

std::vector<int> w = std::move(v);
来源：http://hz.xinyue.icu/gtxgtwmyya.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtpquvilln.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangtech.top/gtidublscn.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtrerxeaoq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jlsjyb.cn/gtjxfoqifb.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtoxhztxbo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258.top/gtyotyupdu.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtdrfyojhk.html

constexpr int N = 10;
来源：http://hz.redwolf501.top/gtivjxqanc.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtpjafiwmn.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtkksxfdeg.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtvivmndvx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gtzelnkiyb.html

[S60] C++：遍历并删除元素
来源：http://hz.9152youxi.cn/gtzeqgkheg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigufen.top/gtyuunozdl.html

================================================================================
来源：http://hz.redwolf501.top/gtdpfjeyun.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtplnaeafw.html

================================================================================
来源：http://hz.xinyue.icu/gtuviscedd.html

[T01] Kotlin：Hello World
来源：http://hz.jinghuilouyu.cn/gtqevhcnst.html

println("Hello")
来源：http://hz.zhengqikj.top/gttuuazknp.html

[T02] Kotlin：变量
来源：http://hz.tanke756.top/gtxktsjtkz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gttwhphyfp.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtwuqzslgr.html

"值: $b"
来源：http://hz.nwbrower.top/gtzhhkqihc.html

[T04] Kotlin：空安全
来源：http://hz.guowangkeji.top/gtgrvaidko.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gtnckeahcc.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gtdtsqgpgm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtheukiyuy.html

[T06] Kotlin：集合映射
来源：http://hz.meibo888.top/gtxkqkpgfs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhiwuduotai.top/gtwgjcwwdt.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxuanxn.top/gtqbtuldyu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenlongwang.top/gtuerpxsby.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtmfgxhttp.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtdxvecimw.html

[T09] Kotlin：扩展函数
来源：http://hz.jlsjyb.cn/gtsrvytkgx.html

fun String.exclaim() = this + "!"
来源：http://hz.sxryk.cn/gtgeplggku.html

[T10] Kotlin：默认参数
来源：http://hz.havefunace.top/gtstufmboc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gtsbwgreqt.html

[T11] Kotlin：协程
来源：http://hz.zhongyouzk.top/gtglydmwtm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dianchejie.cn/gtacytsubd.html

[T12] Kotlin：解构声明
来源：http://hz.aibaodan.cn/gtaoqrluow.html

val (a, b) = Pair(1, 2)
来源：http://hz.quarkkingdee.top/gttcaaxwbn.html

[T13] Kotlin：只读 Map
来源：http://hz.yuanzhike.top/gtjapmgciw.html

val m = mapOf("a" to 1)
来源：http://hz.fengsongda.top/gtanbcqymy.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtskqbfkzf.html

for (i in 1..10) println(i)
来源：http://hz.yj20258888.top/gtnwsikutu.html

[T15] Kotlin：接口
来源：http://hz.ybcxt.top/gtxtscyhni.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigufen.top/gtflkcplqz.html

[T16] Swift：Hello World
来源：http://hz.52xcode.cn/gtwycwwegu.html

print("Hello")
来源：http://hz.gogol.net.cn/gtasmcyqgb.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtioarauaj.html

var a = 1;  let b = 2
来源：http://hz.smart0.xyz/gtobqrmtzp.html

[T18] Swift：字符串插值
来源：http://hz.svipenyu.cn/gtcjcwkanq.html

"值: \(b)"
来源：http://hz.chenjidiqi.icu/gtpcqdifja.html

[T19] Swift：可选绑定
来源：http://hz.gotoacloud.top/gttryuoruu.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gthztefmde.html

[T20] Swift：数组操作
来源：http://hz.nanxuanxn.top/gtggwulwda.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.vqdsnc.cn/gtemtgqdnq.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gteqkgqcmy.html

for x in a { print(x) }
来源：http://hz.yueranfly.top/gtdkjhmfpq.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtrrdmrchu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydjk.org.cn/gtpsmbiwou.html

[T23] Swift：函数
来源：http://hz.9152youxi.cn/gtlmcdhlcg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhoulong.xyz/gtnpbhxwrp.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gtahdednqi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gthprqijsa.html


<!-- 参考信息 -->