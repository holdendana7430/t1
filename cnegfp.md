代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtrqoadbao.html

[R34] 退出时清理
来源：http://hz.hysaishi.cn/gtfikwyhdd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtzpvdfpid.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtongdgaan.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gttepgvyfe.html

[R36] 并发执行多个任务
来源：http://hz.gotoacloud.top/gtzgmrfhau.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.havefunace.top/gtektxtryd.html

[R37] 把输出赋给变量
来源：http://hz.zhiwuduotai.top/gtyxpfokjx.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtunnkwuki.html

[R38] 管道串联
来源：http://hz.gogol.net.cn/gtmohfuvod.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtmuousnfp.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtximyjdgh.html

cmd > out.log 2>&1
来源：http://hz.xuetiantiany.cn/gtctdpjwdx.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtifnsaoyp.html

echo "log" >> out.log
来源：http://hz.yuxming.cn/gtlnwqaois.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtiafgjiqh.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtiefokkij.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtciahclfd.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtbycppdvg.html

[R43] 按名字查找文件
来源：http://hz.c1oappe.top/gtqibmrzst.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtzeizukqh.html

[R44] 按修改时间查找
来源：http://hz.daxiang520.top/gtrnslkpsu.html

find . -mtime -7 -type f
来源：http://hz.hammf.cn/gthikuwcqd.html

[R45] 批量删除
来源：http://hz.ivvv.top/gtgfdxepwd.html

find . -name "*.tmp" -delete
来源：http://hz.pycfn.com/gtrsiukzzp.html

[R46] 递归替换文件内容
来源：http://hz.jqgfzy.top/gtmabzddle.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtoirpzjss.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtzschbsds.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtjydalvoo.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtchmfacvx.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gtdtxwrwar.html

[R49] awk 带条件
来源：http://hz.quarkkingdee.top/gthnilrama.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtnqgjytnr.html

[R50] awk 求和
来源：http://hz.xuanzx.com/gtfgwgrwcx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtocnllzve.html

[R51] 排序去重取前几
来源：http://hz.hnqzz.top/gtflenrgxx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hongshengwenyu.top/gtnirkfoay.html

[R52] 统计行数
来源：http://hz.shangyingyoupin.top/gtjoxdmmuv.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtkteyyjiy.html

[R53] 查看文件头与实时尾
来源：http://hz.cucudq.cn/gtyozvrmsd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtbaupohrs.html

[R54] 比较两个文件
来源：http://hz.yj202588.top/gtxzzbfdxl.html

diff a.txt b.txt
来源：http://hz.feifeiyinyue.top/gtahwysqhj.html

[R55] 压缩与解压
来源：http://hz.andypj.xyz/gtuokzpmvf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cheryme.top/gtgdifwtth.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtvkugamcd.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtrzesbemj.html

[R57] 远程执行命令
来源：http://hz.ywan-chungtsiang.top/gterhdxkcn.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtocwjphgx.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtpfnxaidj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtfawatidu.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtjymlxfhv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtgmaxuezj.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtrtwxqduk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.9152youxi.cn/gtcclyruek.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtealuuift.html

df -h;  du -sh *
来源：http://hz.svipenyu.cn/gtrwqahsuu.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtzlfcfgov.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtahcgwrkd.html

[R63] 内存与进程
来源：http://hz.ivvv.top/gtebgzcrsb.html

free -h;  ps aux | grep nginx
来源：http://hz.iojbl.cn/gtxjdiyfym.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtcyyhmuet.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtvdqfrqlq.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtzfakvajx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.smart0.xyz/gtjnkxynwz.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtayvlqcca.html

crontab -e;  crontab -l
来源：http://hz.zhiwuduotai.top/gttybzzhhf.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gtrpnrtfdi.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtnryjxixi.html

[R68] 计算文件校验值
来源：http://hz.smart0.xyz/gtjlqepufz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuxming.cn/gtsihlwicn.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtlseabgkv.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtluqomwft.html

[R70] 时间戳与互转
来源：http://hz.52xcode.cn/gtjxsknaep.html

date +%s;  date -d @1700000000
来源：http://hz.bjfxy.top/gtovezauok.html

[R71] 日期格式化
来源：http://hz.cheryme.top/gtiqarcksj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gtzlhyafxs.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gttmvqqmqe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtykkuktkg.html

[R73] 分割大日志
来源：http://hz.pengpengdd.cyou/gtfeapwnim.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtotkjwszg.html

[R74] 批量重命名
来源：http://hz.chenzaomai.com/gtnmnyopaa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtofaqoftr.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gtmmzunshu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guannengcc.top/gtepimdejw.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtatoyyosb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtmoohslaf.html

[R77] 读取用户输入
来源：http://hz.yongpay.top/gtgegysnzy.html

read -rp "请输入: " ans
来源：http://hz.zhijiandao.cn/gtvzucmhgi.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gtiqctkbrx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtqdqbihbb.html

[R79] 解析命令行选项
来源：http://hz.cheryme.top/gtmqmnlqdc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gttwokmuty.html

[R80] 查看脚本执行耗时
来源：http://hz.zhoulong.xyz/gtkfijwqad.html

time ./run.sh
来源：http://hz.ydzc1.top/gttgeprdsg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsijaqsma.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtmwsdtyie.html

================================================================================
来源：http://hz.daria6918.cn/gtaahllaft.html

[S01] C：Hello World
来源：http://hz.pycfn.com/gtonzjwzwg.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtbopzilmo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.birdmap.top/gtvnrgcmaf.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtkhtvpddw.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gtnrdrjqrr.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gtumwkmutq.html

int x; scanf("%d", &x);
来源：http://hz.cashguo.top/gtvekpxruk.html

[S04] C：字符串复制
来源：http://hz.zycfv.cn/gttsaxesqo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtuycykiwy.html

[S05] C：字符串长度
来源：http://hz.sweek.top/gtgsfxrqbh.html

strlen(s)
来源：http://hz.sweek.top/gtdcaklhhd.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gteazwbbzh.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtjyzahigh.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtzjafnnws.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinghuilouyu.cn/gtvhqbuzuv.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtsebsitzm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtigkzfdig.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtlqfgqgcj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtsxzrecfm.html

[S10] C：指针与解引用
来源：http://hz.haohaochexian.top/gtwgrjthcz.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gtywgsrbuo.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtynpookeh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtsfilngnd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtplvmzbgg.html

fclose(f);
来源：http://hz.xinyue.icu/gtdacitfci.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtmyvevpvr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhijiandao.cn/gthmveiwjr.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtwwusqviz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.52xcode.cn/gtsrdijoyy.html

[S14] C：枚举
来源：http://hz.iojbl.cn/gtyblrfmxp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj202588.top/gtvlrbkcoq.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtekiufjif.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtzjfprhes.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtotgsvicj.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gthpmunzxr.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtaurzuymq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shuidangran.top/gtcfnmeowy.html

[S18] C：命令行参数
来源：http://hz.yj20258.top/gtdijbkyig.html

int main(int argc, char **argv)
来源：http://hz.cqqwz.cn/gthuqxkhsm.html

[S19] C：快速排序
来源：http://hz.yvedp.cn/gtuehwdzht.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtjrziyhfg.html

[S20] C：二分查找
来源：http://hz.kuanghao11.cn/gtnlvzgxpy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtyhzznqma.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtmcavpodn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gtvedqsbgy.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtkiwoxneq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gtktotfhpk.html

[S23] C：随机数
来源：http://hz.yuxming.cn/gtogvzpdfa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.havefunace.top/gtwrxfvksz.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtqnyryxhq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtnrpaxnmi.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtydbkysve.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtjwpeeytb.html

[S26] C：内存清零
来源：http://hz.dashuyun.cn/gtjckwsmrr.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtggmabsqd.html

[S27] C：定义常量
来源：http://hz.yongpay.top/gtjjutuuxb.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtzbrietue.html

[S28] C：静态变量
来源：http://hz.316326.xyz/gtgwxiohsw.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtzakoelqo.html

[S29] C：变参函数
来源：http://hz.shuidangran.top/gtscabvzer.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtmdvyqdyu.html

[S30] C：头文件保护
来源：http://hz.sysykeji.top/gtnyszyczj.html

#ifndef X_H
来源：http://hz.hongshengwenyu.top/gtyvksebzi.html

#define X_H
来源：http://hz.zhoulong.xyz/gtzrtrjkid.html

#endif
来源：http://hz.vqdsnc.cn/gtocidtfuo.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtetreibgk.html

#include <iostream>
来源：http://hz.smart0.xyz/gtcqbjhbvh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shangyingyoupin.top/gtfrbhvqzw.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gthmrwwcci.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtfabfinbh.html

[S33] C++：vector 增删
来源：http://hz.kuanghao11.cn/gtkuayfsuq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhengqikj.top/gtclapxcjf.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtfjrzkfib.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnqzz.top/gtbuphluoa.html

[S35] C++：map
来源：http://hz.shanyushiyangtech.top/gtspplslnr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtqsaesnhe.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtxofkmuxk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtzalwgizm.html

[S37] C++：set
来源：http://hz.316326.xyz/gtjhccolvt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtxkdszung.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gtxuwnlecv.html

std::sort(v.begin(), v.end());
来源：http://hz.hnxiangtu.top/gtbkufwaik.html

[S39] C++：自定义比较器排序
来源：http://hz.daria6918.cn/gtnkxuiemr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gtuwtozqbk.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtiuiijvcr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtslwwmvnh.html

[S41] C++：类与构造函数
来源：http://hz.iojbl.cn/gtwiopbmta.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtvezdjtoz.html

[S42] C++：继承与虚函数
来源：http://hz.0kj1m.cn/gttmqpjesc.html

class B : public Base { public: void f() override {} };
来源：http://hz.ppjwa.cn/gtlobxjsin.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtfepbvqci.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhoulong.xyz/gteexmwnxv.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gtolcskzpi.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtjkzwpnkw.html

[S45] C++：lambda
来源：http://hz.hfpthk.cn/gtfnvhahoo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtabcmnzrc.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtzuvbzrcy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigufen.top/gtaivbffrs.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtlovqevfh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gttjpsenez.html

[S48] C++：逐行读文件
来源：http://hz.dianchejie.cn/gtqqtsxnov.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hywenlv.cn/gtxvbbbptj.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtizvdzmad.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtjudqyymy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigufen.top/gtlgoxmdmy.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtjcrqfdts.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhixingplan.top/gtufypvsnd.html

[S51] C++：显式类型转换
来源：http://hz.cdnleiting.top/gthnrbucta.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtcolehcvh.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtarjrziik.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtzcnnwlso.html

[S53] C++：移动语义
来源：http://hz.daxiang520.top/gtsibcxvtb.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtazbwehel.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gttczqbfny.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuxming.cn/gtrfhzstws.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtdbzphtsk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yanxiufei.cn/gtbrvwkbra.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtjiedqoon.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gtaoipogpr.html

[S57] C++：编译期常量
来源：http://hz.ybcxt.top/gtgzqtxweg.html

constexpr int N = 10;
来源：http://hz.feifeiyinyue.top/gtaouhnyhi.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gttusdzvhq.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtnjcetwxr.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gttrlwsolx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtdnjhsown.html

[S60] C++：遍历并删除元素
来源：http://hz.guannengcc.top/gtqehcpbaf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtdpxzjhmn.html

================================================================================
来源：http://hz.316326.xyz/gtlogzvbjr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtrkdnjegl.html

================================================================================
来源：http://hz.cucudq.cn/gtvvhvlfgz.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gtswhpygit.html

println("Hello")
来源：http://hz.daria6918.cn/gtoicjuvgb.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtoaxpbzia.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangshuangyany.cn/gtmbtwvmjo.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtsstqzwlf.html

"值: $b"
来源：http://hz.yueranfly.top/gttocqybfs.html

[T04] Kotlin：空安全
来源：http://hz.jinghuilouyu.cn/gtosekrxsa.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtmcnagdgf.html

[T05] Kotlin：when 表达式
来源：http://hz.cheryme.top/gtbblcpdhq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtxtddxydl.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtlrujsdwb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtdshlbrom.html

[T07] Kotlin：集合过滤
来源：http://hz.chenjidiqi.icu/gtzevuhszf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtgqgfzeon.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtytibxnne.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtcjtcvwbj.html

[T09] Kotlin：扩展函数
来源：http://hz.haohaochexian.top/gtqfyuunlc.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtgwtbjxnx.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtiavurzdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtbrpkmfwl.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtwhgcroyy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtzzwccume.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtkujbvvtm.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gtcxlukxnv.html

[T13] Kotlin：只读 Map
来源：http://hz.tianlin.xyz/gtigjjyayg.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtwcsuvmue.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtrrbsdnav.html

for (i in 1..10) println(i)
来源：http://hz.ydzc1.top/gtdtonhdbl.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtzadsjfut.html

interface Shape { fun area(): Double }
来源：http://hz.bjfxy.top/gtqbcoplya.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtlpjfvkov.html

print("Hello")
来源：http://hz.xuanzx.com/gtmseinhng.html

[T17] Swift：变量与常量
来源：http://hz.xziqi.cn/gtxsmnupwc.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtluhpnsxb.html

[T18] Swift：字符串插值
来源：http://hz.tanke756.top/gtmrmcdscy.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtzgmmiiab.html

[T19] Swift：可选绑定
来源：http://hz.cheryme.top/gtzdremigb.html

if let n = opt { print(n) }
来源：http://hz.hfpthk.cn/gtafnuiits.html

[T20] Swift：数组操作
来源：http://hz.c1oappe.top/gtomskidxv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuetiantiany.cn/gtxwyfuktj.html

[T21] Swift：遍历
来源：http://hz.bjfxy.top/gtublksbmh.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtrvkfrinm.html

[T22] Swift：字典
来源：http://hz.ydjk.org.cn/gtcrftcyto.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhiwuduotai.top/gtfctusvcb.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gttqltqxez.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtzkooyqpa.html

[T24] Swift：闭包
来源：http://hz.yuxming.cn/gtyamubvfg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yanxiufei.cn/gtqzqlfuvb.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtypdhcsgm.html

struct P { var x: Int }
来源：http://hz.ydjk.org.cn/gtlaybdlgy.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gteqrvarrj.html

class A: Base { override func f() {} }
来源：http://hz.smart0.xyz/gtqcptjidj.html

[T27] Swift：错误处理
来源：http://hz.9152youxi.cn/gtchdzujya.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gtwjmvvjro.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtazpzenqq.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gtveuuzsql.html

[T29] Swift：guard 提前返回
来源：http://hz.hfpthk.cn/gtuhxbilkf.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtyodksrwd.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gtqqslfjso.html

protocol Shape { func area() -> Double }
来源：http://hz.cashguo.top/gtgthxqkyl.html

[T31] Lua：Hello World
来源：http://hz.hongshengwenyu.top/gtxqklyfxh.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtzirprrlg.html

[T32] Lua：局部变量
来源：http://hz.aibaodan.cn/gtxhawdtur.html

local a = 1
来源：http://hz.yongpay.top/gtvuyniyfv.html

[T33] Lua：表（数组）
来源：http://hz.chenjidiqi.icu/gtdmitgoiw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtlkqieqlh.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtkdqqxsve.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhoulong.xyz/gtyjuaavyo.html

[T35] Lua：字典表
来源：http://hz.andypj.xyz/gtvnxcvpsf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zdqjudy.top/gtvhciutyd.html

[T36] Lua：函数
来源：http://hz.aibaodan.cn/gtkvsvquya.html

function add(a, b) return a + b end
来源：http://hz.yonumen.top/gtlwrnbajd.html


<!-- 参考信息 -->