代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hammf.cn/gtsyhpzvgl.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtcdybvpqu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cashguo.top/gtshmwjywv.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtmepldjfb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtprtgdstr.html

[R26] 命令替换
来源：http://hz.smart0.xyz/gtuqwdpfdy.html

now=$(date +%F); echo "$now"
来源：http://hz.jinghuilouyu.cn/gtkxvetrwo.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtcgijhyvd.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtajjijrue.html

[R28] 浮点运算
来源：http://hz.cashguo.top/gtsbdgvlub.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtcvgysgah.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtqyxzsbyu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtuzreopme.html

[R30] 函数返回状态码
来源：http://hz.ydjk.org.cn/gtfuxoalli.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtifvpdcgo.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtrmufupzj.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtoqwbsspp.html

[R32] 参数个数校验
来源：http://hz.zhiwuduotai.top/gtosbkeyvl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtfvehhasm.html

[R33] 捕获错误并提示行号
来源：http://hz.hnxiangtu.top/gtbpbtpwsw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hfpthk.cn/gtlrhvuwgc.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtxuqcchry.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtqehlsfgj.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtvlpasqtp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtixiggemd.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtdfizcbei.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shzxlz.cn/gteyvncxsq.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtfccwcmol.html

files=$(ls -1)
来源：http://hz.zhengqikj.top/gtdwaamsjm.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtlnsulcdu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtdcmmiolr.html

[R39] 重定向标准输出与错误
来源：http://hz.fzhhl.top/gtfmquvevi.html

cmd > out.log 2>&1
来源：http://hz.yangfankeji.com/gtmfzvibgj.html

[R40] 追加写日志
来源：http://hz.jyoumei.cn/gtdxvizsnt.html

echo "log" >> out.log
来源：http://hz.xingfuxueyuan.xyz/gtxnazsrir.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtnpawhhua.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtvtuujkbb.html

[R42] 输入重定向
来源：http://hz.cucudq.cn/gtnneytigy.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtqbylcfsv.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtnotsgbpe.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gttoftacyi.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gtrnhkrjky.html

find . -mtime -7 -type f
来源：http://hz.hfpthk.cn/gtkaqvlzmz.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtcrzfjpum.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtamfvxmnc.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtquipcieb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gttjvgewtj.html

[R47] sed 单行替换
来源：http://hz.zhaomingkeji.xyz/gtotjbjqup.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.snrcjt.cn/gtllrvqdku.html

[R48] awk 取指定列
来源：http://hz.xinyue.icu/gtgrghnwwt.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gttmsscxpg.html

[R49] awk 带条件
来源：http://hz.xinyue.icu/gtdimhkrye.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.9152youxi.cn/gtllgsozwz.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gtsxsciine.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtnlcncaxf.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtpusuibaj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtxmltrgjh.html

[R52] 统计行数
来源：http://hz.feifeiyinyue.top/gtoitgzzzp.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtefkzxtmd.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gtfdyihrur.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtfsqcmwdq.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gtvwkwufdm.html

diff a.txt b.txt
来源：http://hz.bjfxy.top/gtjwucxzaa.html

[R55] 压缩与解压
来源：http://hz.hfpthk.cn/gtawnhnyaz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sysykeji.top/gtozhrhmgb.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtvnqojydd.html

scp file user@host:/path/
来源：http://hz.jinghuilouyu.cn/gtoaeshbqb.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtifxxwjhw.html

ssh user@host 'uptime'
来源：http://hz.0kj1m.cn/gtnavvjtsi.html

[R58] 下载文件
来源：http://hz.hammf.cn/gtncfokrws.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuetiantiany.cn/gtiinfucfu.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gtndkmlmqk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gthcpkebev.html

[R60] 只看 HTTP 状态码
来源：http://hz.daxiang520.top/gttjkcyobn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuanzx.com/gtpvubskwf.html

[R61] 磁盘占用
来源：http://hz.quarkkingdee.top/gtvlgnrgeo.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtukkzbzuk.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtvvjavvhe.html

du -ah . | sort -rh | head -10
来源：http://hz.cheryme.top/gtgemdundo.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtvudfdoyf.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtudoehmze.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtbocyasti.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangtech.top/gtnlylllct.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtywyohkxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtmdzzddcf.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gtanhrycni.html

crontab -e;  crontab -l
来源：http://hz.jianghu66.top/gtkkjtrckj.html

[R67] 生成随机十六进制串
来源：http://hz.sysykeji.top/gthhjrmzhk.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtdfjfmlwf.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtzvlcmxxb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtxyxpdgvr.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtpyjgzugg.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gthocxelze.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtyyvswaje.html

date +%s;  date -d @1700000000
来源：http://hz.0kj1m.cn/gtmnrspdui.html

[R71] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtnuegxjgl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtahjigpjs.html

[R72] 等待端口就绪
来源：http://hz.zhijiandao.cn/gtbkmgebzr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cqqwz.cn/gtwenbsaat.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gtytbmqwck.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtrapqssra.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtckbhzfwu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydzc1.top/gtgujurabp.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtzhlxduil.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yonumen.top/gtotbtxxyv.html

[R76] 使用临时文件
来源：http://hz.gzhubu.top/gtgwzcwbhr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtlkcotigq.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gtyvealrca.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtibdfxqot.html

[R78] 交互式菜单
来源：http://hz.ivvv.top/gtruxobxig.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtztnrcbdp.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangtech.top/gtrbmeyqez.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gzhubu.top/gtftutpuai.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtyfjrdrng.html

time ./run.sh
来源：http://hz.havefunace.top/gthdhkettz.html

================================================================================
来源：http://hz.daria6918.cn/gtopbziwww.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtqrdcxzon.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvbjtuchg.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gtjclfkjtc.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtusdhqgsh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtkvuiqdin.html

[S02] C：变量与格式化输出
来源：http://hz.pycfn.com/gtbxxxokdx.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gteqqcrvdb.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtwzvujtzy.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtvxgcnikt.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtmyitvkvc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtibbgiygm.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtvzjdibmx.html

strlen(s)
来源：http://hz.tanke756.top/gtaegnwmix.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtedkjkyhu.html

strcmp(a, b) == 0
来源：http://hz.316326.xyz/gtqgbcdygo.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtckaqpjyk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gtfvpaxjcl.html

[S08] C：动态内存分配与释放
来源：http://hz.svipenyu.cn/gtzulyzagd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gthcdjmruv.html

[S09] C：结构体定义与初始化
来源：http://hz.dashuyun.cn/gtnjhwynup.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtjxcjbujx.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtnhainlvk.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtkqqsehxt.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtaykwngqp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fengsongda.top/gtnpwdpedu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtazwfzkmp.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtjrduqbmx.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtzewpfxuy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yongpay.top/gtaahwwbgf.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gttvjrtbcm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gotoacloud.top/gtaslfaauy.html

[S14] C：枚举
来源：http://hz.yongpay.top/gtwbvhudty.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gtmkmbkrfe.html

[S15] C：类型转换
来源：http://hz.9152youxi.cn/gtovnzohfd.html

(double) a / b
来源：http://hz.xylfe.cn/gtjzeuadio.html

[S16] C：位操作置位
来源：http://hz.shzxlz.cn/gtlmsznqnq.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtailozbur.html

[S17] C：安全拼接字符串
来源：http://hz.fzhhl.top/gtkrxzrjty.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtlpswtdmb.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtvsyjjydd.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gttxlhvhxn.html

[S19] C：快速排序
来源：http://hz.chenzaomai.com/gtarsybkvr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtnzferfah.html

[S20] C：二分查找
来源：http://hz.sweek.top/gtpspoyxnb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtligmbqha.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtcoolcgnb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gttzpzdqzc.html

[S22] C：字符串转数字
来源：http://hz.yonumen.top/gtosvqnpcu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shuidangran.top/gtxogehnsq.html

[S23] C：随机数
来源：http://hz.jinqigufen.top/gtmqasoqaw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.aizwys.cn/gtbroxgisn.html

[S24] C：获取本地时间
来源：http://hz.svipenyu.cn/gtxolrbxqe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.birdmap.top/gtduxvfapr.html

[S25] C：内存拷贝
来源：http://hz.yanxiufei.cn/gthymygrvz.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtxysbdynn.html

[S26] C：内存清零
来源：http://hz.guowangkeji.top/gtjhzjqgku.html

memset(a, 0, sizeof a);
来源：http://hz.hywenlv.cn/gtsuhatskx.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtehsdraqk.html

const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtrocdxlba.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtwhtwgcxw.html

static int counter = 0;
来源：http://hz.smart0.xyz/gtiztrofoc.html

[S29] C：变参函数
来源：http://hz.hywenlv.cn/gtewvxjiun.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtstwbnioo.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtbwwzvpdk.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtjjriwtdk.html

#define X_H
来源：http://hz.andypj.xyz/gtflogmlbw.html

#endif
来源：http://hz.chenzaomai.com/gtgnbigrps.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtwfiwbalc.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtgblkhlzw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtefpsmwar.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtjvxnltei.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtlxmwdbgg.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtlwapkkkt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.vqdsnc.cn/gtewqfkcqe.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gtcpekgbxu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnxiangtu.top/gtdinuailq.html

[S35] C++：map
来源：http://hz.birdmap.top/gtfygwxsbm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtwozsnfhu.html

[S36] C++：unordered_map
来源：http://hz.zdqjudy.top/gthhainvxz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtfdmzedkg.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtpzmoeguh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtfuxywjcy.html

[S38] C++：排序
来源：http://hz.sufxvd.cn/gtbkqjddpd.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtiugutvzq.html

[S39] C++：自定义比较器排序
来源：http://hz.guowangkeji.top/gtymgpwsft.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sweek.top/gtudevnfdh.html

[S40] C++：查找元素
来源：http://hz.zhongyouzk.top/gtyoykuyvs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gtkdsziwys.html

[S41] C++：类与构造函数
来源：http://hz.svipenyu.cn/gtokidbkhr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.redwolf501.top/gtjutpatpv.html

[S42] C++：继承与虚函数
来源：http://hz.pengpengdd.cyou/gtfaapziav.html

class B : public Base { public: void f() override {} };
来源：http://hz.snrcjt.cn/gtxtfwqhoc.html

[S43] C++：智能指针
来源：http://hz.yuanzhike.top/gtnaducwva.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtftiqpoql.html

[S44] C++：引用传参
来源：http://hz.wangdashe.top/gtggygqiah.html

void inc(int &x) { ++x; }
来源：http://hz.zhaomingkeji.xyz/gtfpnzpykf.html

[S45] C++：lambda
来源：http://hz.hnqzz.top/gtslyeftdo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gzhubu.top/gtxutpoptv.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtjpdtdcjy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ywan-chungtsiang.top/gtqlsjkwvg.html

[S47] C++：结构化绑定遍历
来源：http://hz.gzhubu.top/gtbncwvjcj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gtmdqseaur.html

[S48] C++：逐行读文件
来源：http://hz.bjfxy.top/gthrttuhis.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinyuanbaomall.cn/gtdxquyhwq.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gtmbasnzwb.html

[S49] C++：写文件
来源：http://hz.zhengqikj.top/gtseotfapv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhiwuduotai.top/gtdhuuruqd.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtkuaridod.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.316326.xyz/gtecmhbtrr.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtfwqoenpl.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtmhqtwyae.html

[S52] C++：const 与 noexcept
来源：http://hz.c1oappe.top/gtujjchnkt.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gttvhltzzj.html

[S53] C++：移动语义
来源：http://hz.nwbrower.top/gtzseomwml.html

std::vector<int> w = std::move(v);
来源：http://hz.birdmap.top/gtjznhrxad.html

[S54] C++：异常处理
来源：http://hz.tian-w.cn/gtdjlamnvb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhijiandao.cn/gtmmcfaleb.html

[S55] C++：结构化绑定
来源：http://hz.cucudq.cn/gtuynredxo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtjqeavuag.html

[S56] C++：optional
来源：http://hz.pengpengdd.cyou/gtjcpsjgxe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtcuczedrp.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtnvpjihqz.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtndomnmta.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gtmvodejbk.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhijiandao.cn/gtuizjkblt.html

[S59] C++：静态断言
来源：http://hz.wangdashe.top/gthxtbiicv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cqqwz.cn/gtvpavyjgt.html

[S60] C++：遍历并删除元素
来源：http://hz.jinghuilouyu.cn/gtvccucngs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daria6918.cn/gtrwfithtw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtordlriuh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtzcbtfnxf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbutyxkxc.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtfvuzkuqj.html

println("Hello")
来源：http://hz.chenzaomai.com/gtmawzitaf.html

[T02] Kotlin：变量
来源：http://hz.jinqigufen.top/gtedxqbdjq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtvqkxzpfw.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtnjalnaan.html

"值: $b"
来源：http://hz.haohaochexian.top/gtmpgafwng.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtommcfhpd.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtsrlzbcxx.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtorirtine.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.andypj.xyz/gtkpmwfgvf.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gtrhkaagek.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtwxxllbja.html

[T07] Kotlin：集合过滤
来源：http://hz.bjfxy.top/gtdjonzvjh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.smart0.xyz/gtulrienjt.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtenbwvyhc.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtnjuqjimo.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangtech.top/gtxmhfckjr.html

fun String.exclaim() = this + "!"
来源：http://hz.kuanghao11.cn/gtpkrboccl.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gttzpxofvw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yueranfly.top/gtpwpxcawh.html

[T11] Kotlin：协程
来源：http://hz.xziqi.cn/gtvqpolfko.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhengqikj.top/gtyvndlgnc.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtbtozoyds.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtshskgyeh.html

[T13] Kotlin：只读 Map
来源：http://hz.52xcode.cn/gtsplznrcr.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gtusgzakgl.html

[T14] Kotlin：循环
来源：http://hz.svipenyu.cn/gtrrmffbzj.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangtech.top/gtkvcbqada.html

[T15] Kotlin：接口
来源：http://hz.hammf.cn/gtnaaurzxl.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtmndiwqbe.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gtxpzwgmkj.html

print("Hello")
来源：http://hz.daria6918.cn/gtfmqnupmy.html

[T17] Swift：变量与常量
来源：http://hz.hongshengwenyu.top/gtnqieglvv.html

var a = 1;  let b = 2
来源：http://hz.zycfv.cn/gtlbwtcwgi.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtlbqzrxxd.html

"值: \(b)"
来源：http://hz.hammf.cn/gtxwvknooi.html

[T19] Swift：可选绑定
来源：http://hz.jinqigufen.top/gtglopfvzq.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtqvyqoclt.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtleueitaq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gtoyjnjtnp.html

[T21] Swift：遍历
来源：http://hz.zhoulong.xyz/gtqhsilesr.html

for x in a { print(x) }
来源：http://hz.fzhhl.top/gtocftwgrq.html

[T22] Swift：字典
来源：http://hz.aizwys.cn/gthflxyevl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xziqi.cn/gtdipysrqn.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtmscfjhyt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.mhx1999.top/gtgakjtqdd.html

[T24] Swift：闭包
来源：http://hz.ehwqpu.com/gtgwagjckz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hfpthk.cn/gtinkyovjm.html

[T25] Swift：结构体
来源：http://hz.yj20258.top/gtjbemgclx.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtiadxwvhp.html

[T26] Swift：类与重写
来源：http://hz.snrcjt.cn/gtewfsossr.html

class A: Base { override func f() {} }
来源：http://hz.yuanzhike.top/gtvbhjfkrv.html


<!-- 参考信息 -->