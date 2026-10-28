代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtioukeumn.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtoxcwhorn.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhixingplan.top/gtyjsmrjmw.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtggzirkac.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtwhyynwqx.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtjysxavsw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtycdshnmj.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtdcflfpdy.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtwvzpisnc.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtlbgzlaia.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cqqwz.cn/gtydoaxpyr.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtgnyezwya.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtfjsfdqqv.html

[R34] 退出时清理
来源：http://hz.yvedp.cn/gtqrifterx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gttbesjlin.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gtaulzsaaa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtfjduawki.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gthetkgqcc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtyzhckutr.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtoexaicas.html

files=$(ls -1)
来源：http://hz.aizwys.cn/gtkdhlytbe.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtdlytukrs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guannengcc.top/gtuierlhvv.html

[R39] 重定向标准输出与错误
来源：http://hz.9152youxi.cn/gtteezptlw.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtbvqzaszd.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtewfpfxcx.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtwwkfdhla.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtmkrvkxyk.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtddcfszof.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtaniuiocy.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtvgnzzsed.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtppjprego.html

find . -name "*.log" -type f
来源：http://hz.gaohongyu789.top/gtgvymiini.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtcznbkabs.html

find . -mtime -7 -type f
来源：http://hz.daxiang520.top/gtnjsdytid.html

[R45] 批量删除
来源：http://hz.ivvv.top/gthdplfhpx.html

find . -name "*.tmp" -delete
来源：http://hz.feifeiyinyue.top/gteucrntvx.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtimyveezt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangshuangyany.cn/gthenkyguw.html

[R47] sed 单行替换
来源：http://hz.ywan-chungtsiang.top/gtkjgpulqn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cheryme.top/gtzmxkryqc.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtmklykglq.html

awk '{print $1, $3}' a.txt
来源：http://hz.svipenyu.cn/gtolreqeaa.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtsqpzksci.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtofzmijqg.html

[R50] awk 求和
来源：http://hz.yj20258888.top/gtuosfwnia.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fzhhl.top/gtssivicar.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtcqkkzjfn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ybcxt.top/gtytpyhqwz.html

[R52] 统计行数
来源：http://hz.jlsjyb.cn/gtjorprhbg.html

wc -l a.txt
来源：http://hz.xingfuxueyuan.xyz/gtxcgizevr.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtlkmyocdu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtalurusii.html

[R54] 比较两个文件
来源：http://hz.chenjidiqi.icu/gtnymzamsn.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gtajaetomd.html

[R55] 压缩与解压
来源：http://hz.jinqigufen.top/gtdhwzrxpk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hammf.cn/gtqqosctkb.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtuqyorxdf.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtlstlijcp.html

[R57] 远程执行命令
来源：http://hz.kuanghao11.cn/gtevmwcpqc.html

ssh user@host 'uptime'
来源：http://hz.xylfe.cn/gtbiatveqx.html

[R58] 下载文件
来源：http://hz.havefunace.top/gtchxority.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gtsuripikj.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gthjyhxuuy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtmhxaecjj.html

[R60] 只看 HTTP 状态码
来源：http://hz.jianghu66.top/gtatbcjynz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtiaiwxefr.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtjlabnadu.html

df -h;  du -sh *
来源：http://hz.316326.xyz/gtamwwcmgu.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtrpjtqpte.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtitljfcbg.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtlildgkdz.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtkqwexxio.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gtdyozsgak.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nanxinkj.top/gtuoaliwhj.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtelwxfgly.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtocpckalm.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtohogavfw.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangkeji.top/gtkagsasxw.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtvyppbnfl.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtxkiacerm.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtttugiknc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtwppmxbjg.html

[R69] 生成随机密码
来源：http://hz.guowangkeji.top/gtxsvvixcj.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtihcnzxjl.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtqilunsjf.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtsvxzyhwq.html

[R71] 日期格式化
来源：http://hz.daria6918.cn/gtwceggadt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gtuaoqpjsb.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtmuwrqlfm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenlongwang.top/gthppqebxs.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtodgnusjq.html

split -l 1000 big.log part_
来源：http://hz.jinqigufen.top/gtqqcykwxu.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtznqmmbtu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtrawmuuda.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtasbmvhbe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gtxyswvbin.html

[R76] 使用临时文件
来源：http://hz.cashguo.top/gtsfvnhwdw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtuptjquja.html

[R77] 读取用户输入
来源：http://hz.kuanghao11.cn/gtaekxvwsh.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtytwckqxh.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtggmxggoy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtquudondg.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtbaxyhldo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtmxxxuvxj.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtooijwncp.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtfeeinljo.html

================================================================================
来源：http://hz.gogol.net.cn/gtebbazwai.html

S. C / C++ 专题
来源：http://hz.jinqigufen.top/gtbvrgntcz.html

================================================================================
来源：http://hz.daxiang520.top/gtglzxejen.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtvbqwqcyq.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gthoxduvte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtvgzfhyln.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gtxymhblob.html

int a = 10; printf("%d\n", a);
来源：http://hz.guannengcc.top/gtgmtcwahm.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtabhqhizq.html

int x; scanf("%d", &x);
来源：http://hz.zhengqikj.top/gtdyddunxf.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtmmtwzfpm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtkfbdnjsi.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtrmttqwei.html

strlen(s)
来源：http://hz.fzhhl.top/gtzyxoapwn.html

[S06] C：字符串比较
来源：http://hz.fzhhl.top/gtikmmxzgz.html

strcmp(a, b) == 0
来源：http://hz.meibo888.top/gtyuuhtqpo.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtfwcxizhr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xingfuxueyuan.xyz/gtkkohyhmp.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtbhnigioy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gtvawkroek.html

[S09] C：结构体定义与初始化
来源：http://hz.yuanzhike.top/gtpegfxxhj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gthvjaqtri.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtsluqbkgu.html

int *p = &a;  *p = 5;
来源：http://hz.shzxlz.cn/gtjgagyhzs.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtqwdpnihm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtgomjjonh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtxyjyzxpn.html

fclose(f);
来源：http://hz.shuidangran.top/gtdsrrmdiz.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtstuinddt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cqqwz.cn/gtfiwtvjud.html

[S13] C：宏定义
来源：http://hz.yonumen.top/gtwhzabbud.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gtfhfbfcfp.html

[S14] C：枚举
来源：http://hz.ydjk.org.cn/gtxkraxvll.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtqyghprep.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtmjknlmeu.html

(double) a / b
来源：http://hz.hnqzz.top/gtnnfiufzn.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtzerpoyus.html

x |= (1 << 3);
来源：http://hz.yongpay.top/gtvaiyxjne.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gtbhbqpyif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shzxlz.cn/gtkomcesvq.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtdccgqxea.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtbwykujvd.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtwzvrxjwn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtrkbubizs.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gthbfwxgye.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtyethzenw.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtypynrtyi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tianlin.xyz/gthacogwby.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtpugjjljf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtpbgyavvn.html

[S23] C：随机数
来源：http://hz.tianlin.xyz/gtesdwgwvm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gtvyzbibyi.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtdeifmzws.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtzjecphsd.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gthhuhfoqi.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtdzwstbcp.html

[S26] C：内存清零
来源：http://hz.tanke756.top/gtmkwklrox.html

memset(a, 0, sizeof a);
来源：http://hz.zhengqikj.top/gtrsciepms.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtovqiahji.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtzdbnpfvz.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtflklqipc.html

static int counter = 0;
来源：http://hz.hongshengwenyu.top/gtwwsopeeu.html

[S29] C：变参函数
来源：http://hz.hywenlv.cn/gtcifvqwhy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtpwkzzjjs.html

[S30] C：头文件保护
来源：http://hz.gogol.net.cn/gtoavwehoi.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtkdgjjxhk.html

#define X_H
来源：http://hz.vqdsnc.cn/gtfmnzxwsy.html

#endif
来源：http://hz.xinyue.icu/gtxbpymmdq.html

[S31] C++：Hello World
来源：http://hz.hammf.cn/gthginzcce.html

#include <iostream>
来源：http://hz.cdnleiting.top/gtvatxsmtc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cheryme.top/gtqpzqtvij.html

[S32] C++：字符串
来源：http://hz.sysykeji.top/gtmoxzjqyx.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtebwbqqxj.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gtihdmhtel.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shangyingyoupin.top/gtkhlydqot.html

[S34] C++：遍历 vector
来源：http://hz.pycfn.com/gtqrmxutoh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shzxlz.cn/gtxghjemzw.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gtnrcjffpv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtvmiwqlvm.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtwbzpudhk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtksfjqndg.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtcwzuxjye.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtslbpiijn.html

[S38] C++：排序
来源：http://hz.sweek.top/gtfbnqityo.html

std::sort(v.begin(), v.end());
来源：http://hz.cqqwz.cn/gtwqsqpumk.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gtnqsgeqbl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangshuangyany.cn/gtbqjzwkym.html

[S40] C++：查找元素
来源：http://hz.gogol.net.cn/gtcjnqmfwr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.52xcode.cn/gtresonufj.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtfnkervxr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gtwadlwdzk.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtffcbsryv.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtlnsgdjsa.html

[S43] C++：智能指针
来源：http://hz.jqgufenzy.top/gtwjugtvxn.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtgdzaqxir.html

[S44] C++：引用传参
来源：http://hz.gotoacloud.top/gtlawbmyea.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtyotsplvq.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtlcjojrfl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtztfgxmtl.html

[S46] C++：函数模板
来源：http://hz.yanxiufei.cn/gtbdjmafdf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtqusptakj.html

[S47] C++：结构化绑定遍历
来源：http://hz.jiagoushi.top/gtqhbjcvft.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.havefunace.top/gtmzopzvfs.html

[S48] C++：逐行读文件
来源：http://hz.nwbrower.top/gtdsovlequ.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gthzhuoyiq.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtxrbdnmwh.html

[S49] C++：写文件
来源：http://hz.zhengqikj.top/gtlkyyauxr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhongyouzk.top/gtsbykgayu.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gteutztmoy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtddtbvhzc.html

[S51] C++：显式类型转换
来源：http://hz.aibaodan.cn/gtgkbzzhgh.html

static_cast<double>(a) / b
来源：http://hz.dianchejie.cn/gtglvgjzqh.html

[S52] C++：const 与 noexcept
来源：http://hz.dianchejie.cn/gtxasaosdq.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gtbpltqabh.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtidroxvkd.html

std::vector<int> w = std::move(v);
来源：http://hz.zdqjudy.top/gtavaugsbe.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtcdcmbzcq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtjgnnfcir.html

[S55] C++：结构化绑定
来源：http://hz.sufxvd.cn/gtfgidlnlu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gtimhufugo.html

[S56] C++：optional
来源：http://hz.feifeiyinyue.top/gtzckravek.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydjk.org.cn/gtkdnxxseh.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtvcdewsru.html

constexpr int N = 10;
来源：http://hz.sweek.top/gtnjsphvyg.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gtfjijzmvm.html

namespace ns { int f() { return 1; } }
来源：http://hz.havefunace.top/gtklwpvntk.html

[S59] C++：静态断言
来源：http://hz.havefunace.top/gtwyfsguig.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.snrcjt.cn/gtwdkdjooq.html

[S60] C++：遍历并删除元素
来源：http://hz.smart0.xyz/gtoxsjnnzs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnxiangtu.top/gtlcctezsl.html

================================================================================
来源：http://hz.cucudq.cn/gtasqmgzcs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtjtigjbvj.html

================================================================================
来源：http://hz.chenlongwang.top/gtycazkkcs.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtuswbuuxc.html

println("Hello")
来源：http://hz.xinyue.icu/gtwyfobuda.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtbchysbqm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj202588.top/gtufwjtgaj.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtionvxiox.html

"值: $b"
来源：http://hz.yonumen.top/gtzzrtyopz.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtpbqkkkdc.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gtayicpyae.html

[T05] Kotlin：when 表达式
来源：http://hz.jinyuanbaomall.cn/gtpbfdfgrs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtwdosbvdr.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtbeehkems.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gtqtmmobku.html

[T07] Kotlin：集合过滤
来源：http://hz.snrcjt.cn/gtrrttadfv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xingfuxueyuan.xyz/gtarjynhjg.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangtech.top/gtotfcojku.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtepsrwuxk.html

[T09] Kotlin：扩展函数
来源：http://hz.svipenyu.cn/gtctsqipaz.html

fun String.exclaim() = this + "!"
来源：http://hz.zhoulong.xyz/gtfeceshwd.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtmlctzilc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.quarkkingdee.top/gtgigfbkff.html

[T11] Kotlin：协程
来源：http://hz.tanke756.top/gtxurluvcn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangtech.top/gtgrgnjuev.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtgapbpskg.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtdcowslro.html

[T13] Kotlin：只读 Map
来源：http://hz.sweek.top/gtiugjmsrd.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtbltgewie.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtksjfbdva.html

for (i in 1..10) println(i)
来源：http://hz.jinghuilouyu.cn/gtistohykg.html

[T15] Kotlin：接口
来源：http://hz.52xcode.cn/gtwjmhuprz.html

interface Shape { fun area(): Double }
来源：http://hz.zhaomingkeji.xyz/gtgpdefoxn.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangkeji.top/gtqjrlrtxs.html

print("Hello")
来源：http://hz.nanxuanxn.top/gtxquqfwch.html

[T17] Swift：变量与常量
来源：http://hz.havefunace.top/gtaubidpuy.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtkughvhwn.html

[T18] Swift：字符串插值
来源：http://hz.daria6918.cn/gtrspdsdah.html

"值: \(b)"
来源：http://hz.guannengcc.top/gtdfmitdxt.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtvreaymwm.html

if let n = opt { print(n) }
来源：http://hz.yuxming.cn/gtimmesqcy.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtkygggngk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtipcmfsdp.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtxkopoqtu.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtoumuhfmn.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtwwvpgezx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtqkychrrp.html

[T23] Swift：函数
来源：http://hz.9152youxi.cn/gtazdpmzqq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhengqikj.top/gtmfvoqfav.html

[T24] Swift：闭包
来源：http://hz.shuidangran.top/gtgbdkrfyl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtcwtkpwaa.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtorbwllgx.html

struct P { var x: Int }
来源：http://hz.jlsjyb.cn/gtuvcvrwro.html

[T26] Swift：类与重写
来源：http://hz.sweek.top/gtfptecxps.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtrevtxpod.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtngvnydiw.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtojzneglr.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtewtmenmd.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gttlkjsdkf.html

[T29] Swift：guard 提前返回
来源：http://hz.0kj1m.cn/gtslfkebrk.html

guard let x = opt else { return }
来源：http://hz.ivvv.top/gtagyyfvmv.html

[T30] Swift：协议
来源：http://hz.yvedp.cn/gtzbivvaex.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtrsvutmhh.html


<!-- 参考信息 -->