代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ppjwa.cn/gtbypiwdfg.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtdwjmdbpx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtodzfjszx.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gttkgrzrtq.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtjglcooai.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gthusglqgu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtebreyxry.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtihqawdlr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yvedp.cn/gtlltvaowq.html

[R34] 退出时清理
来源：http://hz.aizwys.cn/gtnhobikqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtnkvsxqrf.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtvvblmtnt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtwiffwtkf.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtgklhjegl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtocsthbiw.html

[R37] 把输出赋给变量
来源：http://hz.andypj.xyz/gtdptpcmor.html

files=$(ls -1)
来源：http://hz.316326.xyz/gtiqqodktk.html

[R38] 管道串联
来源：http://hz.xingfuxueyuan.xyz/gtqcwxjypd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtwatrvbfk.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtxpnrejjk.html

cmd > out.log 2>&1
来源：http://hz.jyoumei.cn/gtppsdadlg.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtabcdemtx.html

echo "log" >> out.log
来源：http://hz.snrcjt.cn/gtzemdqnbs.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtpiqrtykz.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtjggarorb.html

[R42] 输入重定向
来源：http://hz.ppjwa.cn/gtzqzmwhcx.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gtkqnrzqpn.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtaburufdh.html

find . -name "*.log" -type f
来源：http://hz.kuanghao11.cn/gtmidvgqsk.html

[R44] 按修改时间查找
来源：http://hz.xinyue.icu/gtashuakvj.html

find . -mtime -7 -type f
来源：http://hz.zdqjudy.top/gtgujuukdg.html

[R45] 批量删除
来源：http://hz.hammf.cn/gttbrvwxqy.html

find . -name "*.tmp" -delete
来源：http://hz.gaohongyu789.top/gtcmqarqms.html

[R46] 递归替换文件内容
来源：http://hz.shangyingyoupin.top/gthycfcosk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtuyvctesh.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtfzfcjgfd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtwfltcrmw.html

[R48] awk 取指定列
来源：http://hz.guannengcc.top/gtcwskvoyc.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtjitodzgu.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtvpcwttpz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.andypj.xyz/gtgojfbitf.html

[R50] awk 求和
来源：http://hz.ivvv.top/gttyasthhl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuxming.cn/gtrbkrjuib.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtfxfxqkob.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtfujmohhb.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtatwqbcsz.html

wc -l a.txt
来源：http://hz.yangfankeji.com/gthlbkitlb.html

[R53] 查看文件头与实时尾
来源：http://hz.xuetiantiany.cn/gthoracuuk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gtyvofsaun.html

[R54] 比较两个文件
来源：http://hz.jianghu66.top/gtanrlglvh.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gtvwunsmxm.html

[R55] 压缩与解压
来源：http://hz.ywan-chungtsiang.top/gtxhpgahmi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtwhhtroml.html

[R56] 远程拷贝
来源：http://hz.jinyuanbaomall.cn/gtdwmoznlt.html

scp file user@host:/path/
来源：http://hz.yueranfly.top/gtxyxgjysh.html

[R57] 远程执行命令
来源：http://hz.havefunace.top/gtdjfcxlhd.html

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtsytlkrjp.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtldllppfp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtkbwhrtvb.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtvagxvtyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtkaxoopnf.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtysbwkobo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuanzx.com/gtzjagtdvr.html

[R61] 磁盘占用
来源：http://hz.hysaishi.cn/gtcpqavrwr.html

df -h;  du -sh *
来源：http://hz.jinqigfzy.top/gtpecegzmr.html

[R62] 找最占空间的文件
来源：http://hz.zhijiandao.cn/gtaerudfys.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtqhfovjzc.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtmnesdvjl.html

free -h;  ps aux | grep nginx
来源：http://hz.chenjidiqi.icu/gtzustktmr.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gtyquktkqq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuanzhike.top/gttfrpsrld.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtfjwndgib.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtauednvvg.html

[R66] 定时任务
来源：http://hz.xuanzx.com/gtfvlsuacy.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gttwutkuir.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtnitiutgq.html

openssl rand -hex 16
来源：http://hz.jiagoushi.top/gtllntezwx.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtyjylvuga.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gthgnmgazv.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtwehedrun.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtyswmwbvh.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtfymmkqdi.html

date +%s;  date -d @1700000000
来源：http://hz.jinghuilouyu.cn/gtgpmayauq.html

[R71] 日期格式化
来源：http://hz.fzhhl.top/gtowyzcjol.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ywan-chungtsiang.top/gtajeseelv.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtdfuyeucf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xylfe.cn/gtlwnkbyko.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtdszlxlul.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtzwythrgb.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtezeuuvor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuetiantiany.cn/gticxowenx.html

[R75] 导出环境变量
来源：http://hz.yuxming.cn/gtqvomdyqv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtgazzufvf.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtzbikprkz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtqkdxpajb.html

[R77] 读取用户输入
来源：http://hz.shzxlz.cn/gtirvmcxph.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtgxtnayhy.html

[R78] 交互式菜单
来源：http://hz.redwolf501.top/gtyhbbswgo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtobswmlvk.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtvfhyfudo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangdashe.top/gtcoevauqx.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtgezxvtze.html

time ./run.sh
来源：http://hz.dianchejie.cn/gtfibgfsvj.html

================================================================================
来源：http://hz.cqqwz.cn/gtjifamvrl.html

S. C / C++ 专题
来源：http://hz.jiagoushi.top/gtzcfakbvq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwflxlypd.html

[S01] C：Hello World
来源：http://hz.wangdashe.top/gtwfkisgof.html

#include <stdio.h>
来源：http://hz.jlsjyb.cn/gtbfxxajhd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ybcxt.top/gtdiewyznc.html

[S02] C：变量与格式化输出
来源：http://hz.yj202588.top/gtnsjlueme.html

int a = 10; printf("%d\n", a);
来源：http://hz.tianlin.xyz/gttcgawqbm.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtilewziqo.html

int x; scanf("%d", &x);
来源：http://hz.cheryme.top/gtrzstebdv.html

[S04] C：字符串复制
来源：http://hz.shzxlz.cn/gtlgladmeg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtusmwfjqy.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtyqydpqah.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtvgnbpmyb.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtuxlhkuoe.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtgqrpqvta.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtrztwyico.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuxming.cn/gtcyfpztpz.html

[S08] C：动态内存分配与释放
来源：http://hz.andypj.xyz/gtiscpudrw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gtglekzdfh.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtnqmnnyte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gtqovluozm.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtsrxhiong.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtaegmduvm.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtfggcuang.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gttdbdfjqy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gtsihjgwju.html

fclose(f);
来源：http://hz.tian-w.cn/gtzyrhuzxh.html

[S12] C：写文件
来源：http://hz.quarkkingdee.top/gtiumdlcga.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gttouxogaw.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtgclijoju.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtsgmxctjq.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtdqmmajfd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aibaodan.cn/gtwvlmyczq.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtxbkyxyaw.html

(double) a / b
来源：http://hz.birdmap.top/gtteevdmuh.html

[S16] C：位操作置位
来源：http://hz.jinqigfzy.top/gtcsedtdjy.html

x |= (1 << 3);
来源：http://hz.zycfv.cn/gtbvfkjris.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtmfzdrcav.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtjgdbshhl.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gthheiavug.html

int main(int argc, char **argv)
来源：http://hz.yongpay.top/gtfuikktnh.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gtmoglojgq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtjfqfqeww.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtjtznkpbo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtvsbvydsa.html

[S21] C：字符类别判断
来源：http://hz.kuanghao11.cn/gtkihvxpiq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtehtmvpuj.html

[S22] C：字符串转数字
来源：http://hz.nwbrower.top/gtzxqbkbwx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtuetwcchj.html

[S23] C：随机数
来源：http://hz.shangyingyoupin.top/gtjazsblaa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtgjnwdfzg.html

[S24] C：获取本地时间
来源：http://hz.sweek.top/gtdcbenkgs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtfdlbeyuw.html

[S25] C：内存拷贝
来源：http://hz.tanke756.top/gthfobqure.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtzglfrhfo.html

[S26] C：内存清零
来源：http://hz.xziqi.cn/gtlrcebxwx.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtfsvshkzy.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtvfksclvv.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtnegrdaak.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtcirayewp.html

static int counter = 0;
来源：http://hz.ehwqpu.com/gtajmecucr.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtvrwddxvk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtpbprujzk.html

[S30] C：头文件保护
来源：http://hz.jinqigufen.top/gtxtddrsmy.html

#ifndef X_H
来源：http://hz.mhx1999.top/gtponkchwa.html

#define X_H
来源：http://hz.jinqigfzy.top/gtevocebku.html

#endif
来源：http://hz.yj20258888.top/gtgyotospd.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtrctdfmqd.html

#include <iostream>
来源：http://hz.mhx1999.top/gtfblxlpsc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhixingplan.top/gtfjoeplrs.html

[S32] C++：字符串
来源：http://hz.yj20258888.top/gtkwghjtwi.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtmrxcvzjs.html

[S33] C++：vector 增删
来源：http://hz.zhixingplan.top/gtyyoxppcx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtgoiruihq.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtxtwjerzq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gogol.net.cn/gtphqjgcaq.html

[S35] C++：map
来源：http://hz.yj202588.top/gttirnhxnr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtcispkrso.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gtznauyxhi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtwrrzenkp.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtrmocyxvy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtwuuwesrl.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtlpapynhp.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtmryhpgaa.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gttkftumrj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangkeji.top/gtukmidafx.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtlodsuyla.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtdbnbudsc.html

[S41] C++：类与构造函数
来源：http://hz.hongshengwenyu.top/gtkjkhjqzu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yongpay.top/gtzjyqabsf.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtpqoaeixc.html

class B : public Base { public: void f() override {} };
来源：http://hz.hammf.cn/gttwrpwwuv.html

[S43] C++：智能指针
来源：http://hz.tanke756.top/gtlktwjbxf.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtlebknhte.html

[S44] C++：引用传参
来源：http://hz.316326.xyz/gtjqzyffsz.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gteyvdpjsq.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gthvveoyxr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtylcxuurs.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtcskwzyof.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gtzhdyhckl.html

[S47] C++：结构化绑定遍历
来源：http://hz.jianghu66.top/gtweazptdb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cqqwz.cn/gtagacwkji.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtgduhovrq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gttwyotbwj.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtnwqcrrms.html

[S49] C++：写文件
来源：http://hz.xuanzx.com/gtslqeyhwz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.birdmap.top/gtbdfgpuyk.html

[S50] C++：格式化数字
来源：http://hz.nwbrower.top/gtjgaayeak.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tianlin.xyz/gtwuhberjv.html

[S51] C++：显式类型转换
来源：http://hz.feifeiyinyue.top/gtskxuohyi.html

static_cast<double>(a) / b
来源：http://hz.yuanzhike.top/gtmjpiqdgp.html

[S52] C++：const 与 noexcept
来源：http://hz.jianghu66.top/gtbivlrbtr.html

int size() const noexcept { return n_; }
来源：http://hz.sufxvd.cn/gtnruiwdnu.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtomtwzjxy.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtybzsnxds.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtbudxgfnd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xinyue.icu/gteuvyelis.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gtsdzfpaqt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yangfankeji.com/gtewgevkes.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gtcgpztijp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtrrqlzzqi.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtulntugyy.html

constexpr int N = 10;
来源：http://hz.kuanghao11.cn/gtlvcfmrrh.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtmfzaqlju.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenjidiqi.icu/gtqtptfcgw.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtoipsiqve.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gtdywsuqut.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgfzy.top/gtacofrquu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hywenlv.cn/gtnuexnzxk.html

================================================================================
来源：http://hz.zdqjudy.top/gtligfdcvl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtfbiyugsp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqfmjoqtl.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gtofxpiitf.html

println("Hello")
来源：http://hz.fengsongda.top/gtpfunbafa.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtqelintpr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hfpthk.cn/gtufumlajm.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtgkayopme.html

"值: $b"
来源：http://hz.zdqjudy.top/gtohuewnww.html

[T04] Kotlin：空安全
来源：http://hz.yuxming.cn/gtonbncams.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gtaqnbojnt.html

[T05] Kotlin：when 表达式
来源：http://hz.xuetiantiany.cn/gtjtqtjjvw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sweek.top/gtbpsxyzzu.html

[T06] Kotlin：集合映射
来源：http://hz.jiagoushi.top/gtixgfnwfh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtcdnfgezz.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258888.top/gtsfsjiuvm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtptylcvdf.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtyjlgwtqj.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtrlwlvvha.html

[T09] Kotlin：扩展函数
来源：http://hz.cdnleiting.top/gtptxlqjil.html

fun String.exclaim() = this + "!"
来源：http://hz.xziqi.cn/gthchyocpc.html

[T10] Kotlin：默认参数
来源：http://hz.guowangkeji.top/gtgvmpvsxq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258.top/gtngtqyiyu.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtviznbide.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hysaishi.cn/gtbjxxlatg.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtppmvsoqu.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtzyddspmb.html

[T13] Kotlin：只读 Map
来源：http://hz.ydzc1.top/gtrqnyjwuv.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigfzy.top/gtxwmidhhp.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gtksnsozkz.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtttnjzjzf.html

[T15] Kotlin：接口
来源：http://hz.xingfuxueyuan.xyz/gtqypphgjb.html

interface Shape { fun area(): Double }
来源：http://hz.bjfxy.top/gtnojwpiin.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtulgsztwg.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gthdkebffq.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtpqlzdlxq.html

var a = 1;  let b = 2
来源：http://hz.vqdsnc.cn/gtvpbdkbod.html

[T18] Swift：字符串插值
来源：http://hz.yuanzhike.top/gtmxoyxwwq.html

"值: \(b)"
来源：http://hz.ppjwa.cn/gtrnarbwey.html

[T19] Swift：可选绑定
来源：http://hz.jiagoushi.top/gtmkeshbqd.html

if let n = opt { print(n) }
来源：http://hz.nanxinkj.top/gtekspouza.html

[T20] Swift：数组操作
来源：http://hz.xuanzx.com/gtpzzcyvwu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hfpthk.cn/gtyeqprxvd.html

[T21] Swift：遍历
来源：http://hz.jiagoushi.top/gtloxlwrqk.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gtuhncnnbj.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gtipmsaznr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yanxiufei.cn/gtefsarswm.html

[T23] Swift：函数
来源：http://hz.snrcjt.cn/gtdtfcwffs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pycfn.com/gtujuucdwy.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtupdubtcc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258888.top/gthsykdour.html

[T25] Swift：结构体
来源：http://hz.tanke756.top/gtzlinsjdh.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtyksqmuzu.html

[T26] Swift：类与重写
来源：http://hz.xinyue.icu/gtfvgcwwrk.html

class A: Base { override func f() {} }
来源：http://hz.shuidangran.top/gtjxdlsdej.html

[T27] Swift：错误处理
来源：http://hz.cqqwz.cn/gtyzzsdzlv.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtosssmodh.html

[T28] Swift：枚举
来源：http://hz.dianchejie.cn/gtmqwzenpk.html

enum Color { case red, green }
来源：http://hz.daxiang520.top/gtkfuodpzl.html

[T29] Swift：guard 提前返回
来源：http://hz.xingfuxueyuan.xyz/gtgppcrnsl.html

guard let x = opt else { return }
来源：http://hz.sufxvd.cn/gtixyygslm.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtutmdjbov.html

protocol Shape { func area() -> Double }
来源：http://hz.ydjk.org.cn/gtdbgjixco.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtbghwjpxz.html

print("Hello")
来源：http://hz.ybcxt.top/gtaozttpii.html

[T32] Lua：局部变量
来源：http://hz.shuidangran.top/gtemwhthuu.html

local a = 1
来源：http://hz.zhengqikj.top/gtklbxmuqa.html


<!-- 参考信息 -->