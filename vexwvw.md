代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tanke756.top/gtehmxcbfr.html

[R30] 函数返回状态码
来源：http://hz.sxryk.cn/gtdqbcrqim.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yangfankeji.com/gtiptyeezs.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtsgtjijmo.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuanzx.com/gthfdmindd.html

[R32] 参数个数校验
来源：http://hz.xziqi.cn/gtfbotvojf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtkzwwkjxf.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtyruuqytp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhaomingkeji.xyz/gtjxmgjyyn.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtvdpceoou.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtvsklcmnb.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtrmptjvcm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ehwqpu.com/gttjygvsvn.html

[R36] 并发执行多个任务
来源：http://hz.fzhhl.top/gtizaraiom.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gtgmpxbvjy.html

[R37] 把输出赋给变量
来源：http://hz.nanxuanxn.top/gtxwxyuzef.html

files=$(ls -1)
来源：http://hz.mhx1999.top/gtadusmlfs.html

[R38] 管道串联
来源：http://hz.sufxvd.cn/gtddeybebo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuanzx.com/gtmgzmomrs.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtlcuvqjou.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtyeadufdl.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gtgarkspds.html

echo "log" >> out.log
来源：http://hz.tanke756.top/gtlpbhaevf.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gtnlkaihdn.html

cmd >/dev/null 2>&1
来源：http://hz.aizwys.cn/gtrngixcyq.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtvevbtaed.html

wc -l < a.txt
来源：http://hz.dashuyun.cn/gtrimuwbgr.html

[R43] 按名字查找文件
来源：http://hz.chenjidiqi.icu/gtrxulxynn.html

find . -name "*.log" -type f
来源：http://hz.andypj.xyz/gtlldedlut.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtzuvfulgw.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtzhxyxjdj.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtijvrxxoe.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtsjahtwat.html

[R46] 递归替换文件内容
来源：http://hz.shzxlz.cn/gtormtdocq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jiagoushi.top/gtycdtawvf.html

[R47] sed 单行替换
来源：http://hz.xuetiantiany.cn/gtvlgqaxkw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj202588.top/gtfvwrrpor.html

[R48] awk 取指定列
来源：http://hz.gogol.net.cn/gtwywlcsju.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtoemdzhnm.html

[R49] awk 带条件
来源：http://hz.zhaomingkeji.xyz/gtemsghrjr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenlongwang.top/gthnfdxuex.html

[R50] awk 求和
来源：http://hz.c1oappe.top/gtztmzncad.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtwtaomqoo.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtprsixzue.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gtegxasjpb.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtmjqlmbyc.html

wc -l a.txt
来源：http://hz.cdnleiting.top/gteqcjotvb.html

[R53] 查看文件头与实时尾
来源：http://hz.havefunace.top/gtmjuvquib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtiyxumqds.html

[R54] 比较两个文件
来源：http://hz.cashguo.top/gtvcumfpay.html

diff a.txt b.txt
来源：http://hz.gogol.net.cn/gtyzhittcl.html

[R55] 压缩与解压
来源：http://hz.hongshengwenyu.top/gtiaxkxcjv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtldjxcmav.html

[R56] 远程拷贝
来源：http://hz.ywan-chungtsiang.top/gtukrnnyff.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gtwkbtblog.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtbqvjnkwq.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtikgozjcv.html

[R58] 下载文件
来源：http://hz.zhixingplan.top/gtocazvqbg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dianchejie.cn/gtvcugmiey.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtwptaoith.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtastayvxe.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtvndyrgvr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.feifeiyinyue.top/gtnbqepvuy.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtplgsplhr.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtbzymqhab.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtjdzkkpjl.html

du -ah . | sort -rh | head -10
来源：http://hz.zhongyouzk.top/gtwqfvuxup.html

[R63] 内存与进程
来源：http://hz.quarkkingdee.top/gtlcqiqnpd.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtjlwjjztf.html

[R64] 结束进程
来源：http://hz.tianlin.xyz/gtyqcjgrvc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtsqictiho.html

[R65] 查看端口占用
来源：http://hz.feifeiyinyue.top/gtkveoivbp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gttuulwrmo.html

[R66] 定时任务
来源：http://hz.guannengcc.top/gtntbtlcnr.html

crontab -e;  crontab -l
来源：http://hz.ppjwa.cn/gtmffxeauq.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtnaecusqe.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtpxcwytdu.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtyltbfjeb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgufenzy.top/gtughcljxm.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtezwlutdm.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtysscnnxy.html

[R70] 时间戳与互转
来源：http://hz.gogol.net.cn/gtlnsmrhwf.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gtjojaiwit.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtuxxmzkjy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtbnpcserp.html

[R72] 等待端口就绪
来源：http://hz.zhaomingkeji.xyz/gtcskdngpq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtlqvbaibv.html

[R73] 分割大日志
来源：http://hz.yangfankeji.com/gtvxdhlsrp.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gttimriurs.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gtbawkymnc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgfzy.top/gtlapfbxuc.html

[R75] 导出环境变量
来源：http://hz.ppjwa.cn/gtxcmoigrd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gthwrmiufn.html

[R76] 使用临时文件
来源：http://hz.redwolf501.top/gtziquayxh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtrzicmmcq.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gtinqllsxa.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gtymioinka.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtaoplgtsi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gtayfzqhlh.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtcahwrnsw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtiokmplpm.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtqcpvyicr.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtvzdkzxlq.html

================================================================================
来源：http://hz.yueranfly.top/gtjwronidn.html

S. C / C++ 专题
来源：http://hz.hfpthk.cn/gtqglagose.html

================================================================================
来源：http://hz.ehwqpu.com/gtopesfwle.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtybasemzp.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtzbpgztng.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtpexwkcce.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtwrgmomau.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtmrdlekaw.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gtcywwdgnu.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtmeremrfm.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gteqffando.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gttjmxelwu.html

[S05] C：字符串长度
来源：http://hz.pengpengdd.cyou/gtydldxhph.html

strlen(s)
来源：http://hz.jqgufenzy.top/gtvkezhgku.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtbihgaclx.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtnmcfnsaf.html

[S07] C：数组遍历求和
来源：http://hz.dianchejie.cn/gtpjtmnumz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gaohongyu789.top/gtqanmgwrb.html

[S08] C：动态内存分配与释放
来源：http://hz.hnqzz.top/gtlzfuywpt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtzxakvcwm.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gtquzassdb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhixingplan.top/gtuvzhmqor.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtxklvhfiz.html

int *p = &a;  *p = 5;
来源：http://hz.zycfv.cn/gtbonyrdoq.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtihriwkkg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sweek.top/gttceqzunl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtjrveobod.html

fclose(f);
来源：http://hz.wangdashe.top/gtvoetnfvi.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gteynjdnkz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigufen.top/gtvurzxpxa.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtikwiogcf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtivdhkiyp.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtvjytahoi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinghuilouyu.cn/gtgergddbt.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gtevzdvcik.html

(double) a / b
来源：http://hz.chenjidiqi.icu/gtkqraeoop.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtksvrsgaz.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gttkmvvohy.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gttgcsxlzr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.andypj.xyz/gtakzumljh.html

[S18] C：命令行参数
来源：http://hz.yvedp.cn/gtirrtykrq.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtrxtmnqpz.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtucmqaizg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtlrsekvew.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtbfpflqhi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtfgqymvsv.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtmqkcuxxy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtjahdlvli.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtjbahmjzm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhengqikj.top/gtxgejgyub.html

[S23] C：随机数
来源：http://hz.meibo888.top/gthunmutmt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gtaejiiidw.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtebguykij.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jyoumei.cn/gtkzddybzw.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gtwwiamtzo.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtzrmscmol.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtelydwgpc.html

memset(a, 0, sizeof a);
来源：http://hz.xinyue.icu/gtwwgkgbhi.html

[S27] C：定义常量
来源：http://hz.gogol.net.cn/gtcezmgukh.html

const double PI = 3.14159;
来源：http://hz.ydjk.org.cn/gttygbpzql.html

[S28] C：静态变量
来源：http://hz.tian-w.cn/gtvoygcwkx.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtogbkrvuk.html

[S29] C：变参函数
来源：http://hz.shuidangran.top/gtoxseajlw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtjnmqzipo.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtbamvykqv.html

#ifndef X_H
来源：http://hz.zycfv.cn/gtsanqumxu.html

#define X_H
来源：http://hz.chenzaomai.com/gtetaebkoq.html

#endif
来源：http://hz.bjfxy.top/gtuyfplqgz.html

[S31] C++：Hello World
来源：http://hz.andypj.xyz/gtmpqnxffj.html

#include <iostream>
来源：http://hz.fzhhl.top/gthlwsqxdz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.pycfn.com/gtefxklpfx.html

[S32] C++：字符串
来源：http://hz.yanxiufei.cn/gtrvnfokzb.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gtsmkhxjwp.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtchrhuvck.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yvedp.cn/gtjfcqsuvy.html

[S34] C++：遍历 vector
来源：http://hz.xinyue.icu/gtgctgtjis.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuanzhike.top/gtfbnbmumk.html

[S35] C++：map
来源：http://hz.ybcxt.top/gtztfxtwzn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtecsynoqi.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtrritspqv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtslxmytzu.html

[S37] C++：set
来源：http://hz.cheryme.top/gtehjxtxoy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtmlhftrkk.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtuyqfwhau.html

std::sort(v.begin(), v.end());
来源：http://hz.jinqigfzy.top/gtxpaofzlg.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtbnveajxy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gtqtwulwjm.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtndjuvujr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.kuanghao11.cn/gtzbvrglgh.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtpjtomwoc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtygxkqrtx.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtpxhzmqkw.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinghuilouyu.cn/gtvndyiuna.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtjlmtzsgi.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydzc1.top/gtlpppgtws.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtetxabgey.html

void inc(int &x) { ++x; }
来源：http://hz.wangshuangyany.cn/gtirumtuxp.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtklgwwoua.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtgzhozitj.html

[S46] C++：函数模板
来源：http://hz.hysaishi.cn/gtjoukjfbt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gthtwifbjx.html

[S47] C++：结构化绑定遍历
来源：http://hz.hammf.cn/gtdgjojwxq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtgmaptomw.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gtuzrbhzvl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtvmhvnxta.html

while (std::getline(in, line)) { }
来源：http://hz.shzxlz.cn/gtlipoczyn.html

[S49] C++：写文件
来源：http://hz.redwolf501.top/gttodmpcew.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.redwolf501.top/gtevmdsgup.html

[S50] C++：格式化数字
来源：http://hz.ywan-chungtsiang.top/gtzaaqzlaw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenzaomai.com/gthfcidwra.html

[S51] C++：显式类型转换
来源：http://hz.0kj1m.cn/gtuhtbjgnq.html

static_cast<double>(a) / b
来源：http://hz.sweek.top/gtdspbggnr.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtsydlqafz.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258.top/gtxustvkyn.html

[S53] C++：移动语义
来源：http://hz.52xcode.cn/gtszyvbdaa.html

std::vector<int> w = std::move(v);
来源：http://hz.aibaodan.cn/gtndmgyodz.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtjbmbzder.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aizwys.cn/gtuirfzhvv.html

[S55] C++：结构化绑定
来源：http://hz.tianlin.xyz/gtledbewcg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.andypj.xyz/gtaiicesmz.html

[S56] C++：optional
来源：http://hz.cheryme.top/gtuqwxnusz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jiagoushi.top/gthwvciyxc.html

[S57] C++：编译期常量
来源：http://hz.gaohongyu789.top/gtmldmtret.html

constexpr int N = 10;
来源：http://hz.yonumen.top/gtbqosjndm.html

[S58] C++：命名空间
来源：http://hz.xingfuxueyuan.xyz/gtnzjmkami.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gthspujong.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtszsukswa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuetiantiany.cn/gthgqxpfww.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gtlokhnhwi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gteahhxqtt.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmhodlroa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtwrxglwbn.html

================================================================================
来源：http://hz.yj20258888.top/gtdvzmdzud.html

[T01] Kotlin：Hello World
来源：http://hz.shangyingyoupin.top/gtxcgytmdo.html

println("Hello")
来源：http://hz.aibaodan.cn/gtkjobpjdt.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtiptioecb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtbeskejzl.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gtkhqhfana.html

"值: $b"
来源：http://hz.pycfn.com/gtcaognulw.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtcwmknegg.html

val n: String? = null;  n?.length
来源：http://hz.yonumen.top/gtrxkuiogx.html

[T05] Kotlin：when 表达式
来源：http://hz.wangshuangyany.cn/gttatmfeos.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gtmdvnlzcj.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gtkaipbxsi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hysaishi.cn/gttybwdkgf.html

[T07] Kotlin：集合过滤
来源：http://hz.ppjwa.cn/gtdflhymtg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtrishebvv.html

[T08] Kotlin：数据类
来源：http://hz.hongshengwenyu.top/gttatkbnyu.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258.top/gtdjnessei.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtwimroata.html

fun String.exclaim() = this + "!"
来源：http://hz.redwolf501.top/gtsvfwohza.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtmyokeptq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gthzdpqhxw.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtinuaobic.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtskhtwhjl.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtujofkdcq.html

val (a, b) = Pair(1, 2)
来源：http://hz.sxryk.cn/gtkxiabghs.html

[T13] Kotlin：只读 Map
来源：http://hz.yueranfly.top/gtlxqnfwyr.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtclhwxqyb.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtdtsnxlkc.html

for (i in 1..10) println(i)
来源：http://hz.jinqigfzy.top/gtfveuniuz.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtgyiznjwe.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtbzkbqadv.html

[T16] Swift：Hello World
来源：http://hz.iojbl.cn/gthfgmtqfo.html

print("Hello")
来源：http://hz.havefunace.top/gtnnusmmmx.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtbydzjmvc.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtbqovipeu.html

[T18] Swift：字符串插值
来源：http://hz.nanxuanxn.top/gtufzxvhtv.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtcmmqjmdq.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtcnoxgoho.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtwatvzhbc.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtdkumuawg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtyobipezn.html

[T21] Swift：遍历
来源：http://hz.daria6918.cn/gttenpxgxt.html

for x in a { print(x) }
来源：http://hz.pycfn.com/gteuastjvv.html

[T22] Swift：字典
来源：http://hz.yueranfly.top/gtojxrotss.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuetiantiany.cn/gtdhderhtl.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtqjefrsak.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtxcbvflib.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gtpoullrqt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtltiiippp.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtpxvojujp.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtjfsqhqmx.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtdtmbkglh.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtcbzuhywn.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtdsvmwcjo.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtebdhsrjh.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtlpzbtnni.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtaxeppudx.html

[T29] Swift：guard 提前返回
来源：http://hz.chenzaomai.com/gtaxpwwnyx.html

guard let x = opt else { return }
来源：http://hz.jinqigufen.top/gtihnwjjja.html

[T30] Swift：协议
来源：http://hz.aibaodan.cn/gthedpcczr.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtxzgjiftn.html

[T31] Lua：Hello World
来源：http://hz.cdnleiting.top/gtwbamhqss.html

print("Hello")
来源：http://hz.zycfv.cn/gttdwcfpjb.html

[T32] Lua：局部变量
来源：http://hz.jqgfzy.top/gtbcyisyva.html

local a = 1
来源：http://hz.dashuyun.cn/gtbhuypifk.html


<!-- 参考信息 -->