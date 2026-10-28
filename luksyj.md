代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxuanxn.top/gtfnugejug.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtnsarulqb.html

now=$(date +%F); echo "$now"
来源：http://hz.guannengcc.top/gtjoofpwgp.html

[R27] 算术展开
来源：http://hz.gogol.net.cn/gtfysxnbfk.html

echo $((1 + 2 * 3))
来源：http://hz.zhongyouzk.top/gtnheazaqw.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtrbpntrjh.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtykwxrucj.html

[R29] 定义函数
来源：http://hz.zycfv.cn/gtxjvhonsx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tianlin.xyz/gtjndytcgr.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtkyisiokj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dianchejie.cn/gtnyiwogxm.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtehqxmuiq.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtuplqmigm.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gttosfspqx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtmuhlcxhw.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtdtsdzhis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtahtikyef.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtmmtdxzik.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtycinuszs.html

[R35] 后台执行并等待
来源：http://hz.9152youxi.cn/gtmbumskgx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtjxuqesps.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtzmchjsmb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtjioshrop.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtdvdkexwg.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtyootcxvo.html

[R38] 管道串联
来源：http://hz.vqdsnc.cn/gtwdpbqjoo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj202588.top/gtoxztobqx.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtgvirmmpw.html

cmd > out.log 2>&1
来源：http://hz.fengsongda.top/gtbiqnhvcr.html

[R40] 追加写日志
来源：http://hz.ydzc1.top/gtjyqozfqp.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtuxedhjim.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtknknfplk.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtfjclavzq.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtvgbtvpwz.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtzwfhlxwk.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtyqfamrpr.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtegxlfawt.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtlpgsdsdi.html

find . -mtime -7 -type f
来源：http://hz.andypj.xyz/gtjlgmkidd.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtyumlkwof.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtyxyngdoi.html

[R46] 递归替换文件内容
来源：http://hz.iojbl.cn/gtnpsvrdcl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtxysfkjeq.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtimhdpxiw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hywenlv.cn/gtevuxspcz.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtzlpjnvtq.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtsduhluqp.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtbugtetxg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.9152youxi.cn/gtkzjqoszz.html

[R50] awk 求和
来源：http://hz.andypj.xyz/gtzcufqtcn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yanxiufei.cn/gtaavcjeln.html

[R51] 排序去重取前几
来源：http://hz.ivvv.top/gtneukmtzi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtmsolkyfk.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtfuumkfyb.html

wc -l a.txt
来源：http://hz.chenlongwang.top/gtntmciwgh.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtaecnfdvw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.316326.xyz/gtzfocxwtu.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtazkwcxqu.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtenpydgbz.html

[R55] 压缩与解压
来源：http://hz.hfpthk.cn/gtrwhpfguz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtxqwcaltn.html

[R56] 远程拷贝
来源：http://hz.hysaishi.cn/gtlhruicjv.html

scp file user@host:/path/
来源：http://hz.sweek.top/gtjvxbzrvq.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gtczmqwrdh.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtxknlaiqz.html

[R58] 下载文件
来源：http://hz.iojbl.cn/gterrtbojo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtpewzuqlh.html

[R59] 发 POST JSON
来源：http://hz.hammf.cn/gtspquxyfj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtiaccputq.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtiassnxjl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gteqgfevsn.html

[R61] 磁盘占用
来源：http://hz.ywan-chungtsiang.top/gtoxgejrrx.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtiwyexasf.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gthfzkbcgj.html

du -ah . | sort -rh | head -10
来源：http://hz.yongpay.top/gthdwyopzg.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtfktqrgpd.html

free -h;  ps aux | grep nginx
来源：http://hz.iojbl.cn/gtvyjknoar.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gtlfphjhir.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtpixhekho.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtbnuizavu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.pycfn.com/gtaxklhozc.html

[R66] 定时任务
来源：http://hz.quarkkingdee.top/gtaxllczfz.html

crontab -e;  crontab -l
来源：http://hz.chenzaomai.com/gtpcjhzcqa.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtujukzbuj.html

openssl rand -hex 16
来源：http://hz.zhengqikj.top/gtsxvaotsq.html

[R68] 计算文件校验值
来源：http://hz.jinqigfzy.top/gtjbnwjtpv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigfzy.top/gtqncfabtx.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gteyzhcind.html

head -c 16 /dev/urandom | base64
来源：http://hz.ywan-chungtsiang.top/gtqmvhqzmm.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtjfnsqoum.html

date +%s;  date -d @1700000000
来源：http://hz.mhx1999.top/gttjokvjvr.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtyjsfhjgr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtvdmagqai.html

[R72] 等待端口就绪
来源：http://hz.52xcode.cn/gtpzujilnc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aibaodan.cn/gtznpqekzd.html

[R73] 分割大日志
来源：http://hz.kuanghao11.cn/gtreftagtg.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtjhafrhwg.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gttfhwbbdz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cucudq.cn/gtjbvjerfy.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtiihuqaag.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gttxcnqjqf.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtezxqbzhk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtqmlsjfif.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtxquuamaw.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtelrjndvd.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtkmbxkwtk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtbivrtjne.html

[R79] 解析命令行选项
来源：http://hz.xinyue.icu/gtnwnocpnn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtwzidkdet.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtnkxmwitf.html

time ./run.sh
来源：http://hz.yj202588.top/gtaknwwtgi.html

================================================================================
来源：http://hz.yonumen.top/gtcrjznekz.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtdxaltfxl.html

================================================================================
来源：http://hz.shzxlz.cn/gtasoepufu.html

[S01] C：Hello World
来源：http://hz.shanyushiyangtech.top/gtujypsfzs.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gttmhbzwiy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gtauudrwxd.html

[S02] C：变量与格式化输出
来源：http://hz.havefunace.top/gttxamzeud.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtobcwpntt.html

[S03] C：读入整数
来源：http://hz.chenjidiqi.icu/gteclpwczl.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gthbfioojc.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtaiiittgo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cashguo.top/gtwesehkqs.html

[S05] C：字符串长度
来源：http://hz.sxryk.cn/gtcdqkhqfm.html

strlen(s)
来源：http://hz.gaohongyu789.top/gtewpztwao.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtulhhtmjj.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtthprhvne.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtorsftlhc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.birdmap.top/gtcxmozqlh.html

[S08] C：动态内存分配与释放
来源：http://hz.zhijiandao.cn/gtvwyiiyec.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aizwys.cn/gtqccfwfdv.html

[S09] C：结构体定义与初始化
来源：http://hz.snrcjt.cn/gtgyszxycn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtijsxwrve.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtzgyzcqhc.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtwfyjtobm.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtdenkksil.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuanzx.com/gtwvbqwqsd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.snrcjt.cn/gtjyvlbzpy.html

fclose(f);
来源：http://hz.iojbl.cn/gthipcoauv.html

[S12] C：写文件
来源：http://hz.yj202588.top/gtnryechkp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtkxcjuhqm.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtffmfblvf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhengqikj.top/gtitcbppiq.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtxegjivly.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gttodqaqpo.html

[S15] C：类型转换
来源：http://hz.wangshuangyany.cn/gtarvpenpu.html

(double) a / b
来源：http://hz.smart0.xyz/gtfdrmkbci.html

[S16] C：位操作置位
来源：http://hz.daria6918.cn/gtjetxzfmy.html

x |= (1 << 3);
来源：http://hz.52xcode.cn/gthbeksiup.html

[S17] C：安全拼接字符串
来源：http://hz.zhiwuduotai.top/gtftoyjvqm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtaoqbvfkn.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtfuznvjii.html

int main(int argc, char **argv)
来源：http://hz.yongpay.top/gtgebkbrtx.html

[S19] C：快速排序
来源：http://hz.daria6918.cn/gtkdggixhw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gttuhexzjy.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtgkzaafex.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtsbnqlwqn.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gtebmupycu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhoulong.xyz/gtdzlzrgep.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtcizdrzgm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtymktcnsu.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gtdzbdkjgu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yueranfly.top/gtjunmxznn.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtgphojcko.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhaomingkeji.xyz/gtrmilojyk.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gtuwwfcril.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtjrrhdmvq.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gteuxngwxg.html

memset(a, 0, sizeof a);
来源：http://hz.shuidangran.top/gtvqztmjds.html

[S27] C：定义常量
来源：http://hz.vqdsnc.cn/gthaypkcsy.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtubtovucj.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gtjzgtatll.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtsvuwoafo.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtuddyvhya.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhongyouzk.top/gtzeanrsqm.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtvxnrggbv.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtcysgetjd.html

#define X_H
来源：http://hz.hammf.cn/gtsuxagdpq.html

#endif
来源：http://hz.ydjk.org.cn/gtduolomsv.html

[S31] C++：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtvpmjodbm.html

#include <iostream>
来源：http://hz.yj202588.top/gtqxududej.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtitjxpjrs.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtufuhrohv.html

std::string s = "hi";  s += "!";
来源：http://hz.fzhhl.top/gtfwlkgixl.html

[S33] C++：vector 增删
来源：http://hz.hywenlv.cn/gtfxwhfcbr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ivvv.top/gtevthqzls.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtlgnnppdp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pengpengdd.cyou/gttdnbwxyy.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtyzfmmydk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtdbtelgci.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtnvlgopku.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtlqlbmrap.html

[S37] C++：set
来源：http://hz.gzhubu.top/gttqhpqcxo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cdnleiting.top/gtzwhobrgf.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtxixamizs.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtclihtcog.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtpprornql.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gtgddeexjd.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtbrhbfoix.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnxiangtu.top/gtzgybvruj.html

[S41] C++：类与构造函数
来源：http://hz.daria6918.cn/gtonolhfzq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gtwgamavdy.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtjpduazkl.html

class B : public Base { public: void f() override {} };
来源：http://hz.daria6918.cn/gtrjiqwbej.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtnqmulxfw.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtbencrkak.html

[S44] C++：引用传参
来源：http://hz.zhoulong.xyz/gtmvdifrgu.html

void inc(int &x) { ++x; }
来源：http://hz.smart0.xyz/gtqaiqtgky.html

[S45] C++：lambda
来源：http://hz.zhaomingkeji.xyz/gtcgjawkqb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtzddjinrq.html

[S46] C++：函数模板
来源：http://hz.wangshuangyany.cn/gtrwvmcjva.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtfdafizsy.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtdwtvfrgw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtwbtuibtf.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtadbgjpaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gteukpzpvr.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gtwdoltyvg.html

[S49] C++：写文件
来源：http://hz.316326.xyz/gtcupxdqrr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtvmhkwnqu.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtvwubwepb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtftyrgtry.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtnnpmxjvc.html

static_cast<double>(a) / b
来源：http://hz.zdqjudy.top/gtfxxrsudq.html

[S52] C++：const 与 noexcept
来源：http://hz.sweek.top/gtcmlqyvzt.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gtoduwagax.html

[S53] C++：移动语义
来源：http://hz.yuxming.cn/gtamfzilji.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtrzfitgtr.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtyspthtcu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gtpuiepuib.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtfxjkucht.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ehwqpu.com/gtrcxgmkaw.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtdxgagujm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gtoiwfijru.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtttdtqpvw.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtbfbaoynr.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gtnupkfxqn.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtkonnytyd.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtqrmxqvzb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtowteojik.html

[S60] C++：遍历并删除元素
来源：http://hz.yanxiufei.cn/gtenmsqtwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hfpthk.cn/gtcrkcdpvp.html

================================================================================
来源：http://hz.sweek.top/gtylchzikv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.feifeiyinyue.top/gtmhldaqex.html

================================================================================
来源：http://hz.svipenyu.cn/gtvcogznqj.html

[T01] Kotlin：Hello World
来源：http://hz.cashguo.top/gtpkyhjske.html

println("Hello")
来源：http://hz.havefunace.top/gtecyzsqjo.html

[T02] Kotlin：变量
来源：http://hz.yangfankeji.com/gtvghyhceo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.meibo888.top/gtmtxklkch.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtxdwqbmcl.html

"值: $b"
来源：http://hz.snrcjt.cn/gtwzwzbshp.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gtpinvibzg.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtthdovhef.html

[T05] Kotlin：when 表达式
来源：http://hz.tianlin.xyz/gtnfhgzdjn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtipainpfo.html

[T06] Kotlin：集合映射
来源：http://hz.bjfxy.top/gtvfkdkgtz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtmyjhkuwc.html

[T07] Kotlin：集合过滤
来源：http://hz.hnxiangtu.top/gtxetxjlbf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.dashuyun.cn/gtdtgnpvja.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtlkxciopj.html

data class User(val name: String, val age: Int)
来源：http://hz.daxiang520.top/gtyqaubkyx.html

[T09] Kotlin：扩展函数
来源：http://hz.ivvv.top/gtjluzriov.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtcmthikvz.html

[T10] Kotlin：默认参数
来源：http://hz.tian-w.cn/gtaizqwkwv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtozyfukdj.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtzuqlophj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aibaodan.cn/gtqycixqhw.html

[T12] Kotlin：解构声明
来源：http://hz.316326.xyz/gtnqinllky.html

val (a, b) = Pair(1, 2)
来源：http://hz.vqdsnc.cn/gtisbvhqqk.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtezosojul.html

val m = mapOf("a" to 1)
来源：http://hz.cheryme.top/gtfhnkltxs.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gttttnzcak.html

for (i in 1..10) println(i)
来源：http://hz.meibo888.top/gtqhggemcq.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gtwncrmvuy.html

interface Shape { fun area(): Double }
来源：http://hz.hfpthk.cn/gtxftssclh.html

[T16] Swift：Hello World
来源：http://hz.yuxming.cn/gttbsspzub.html

print("Hello")
来源：http://hz.yonumen.top/gtttfyxziw.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gtimowhraf.html

var a = 1;  let b = 2
来源：http://hz.guannengcc.top/gtllabyhpc.html

[T18] Swift：字符串插值
来源：http://hz.daria6918.cn/gtdasqpguu.html

"值: \(b)"
来源：http://hz.yangfankeji.com/gtplyeeenr.html

[T19] Swift：可选绑定
来源：http://hz.yj202588.top/gtuwvbzybd.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtmsearhyb.html

[T20] Swift：数组操作
来源：http://hz.tanke756.top/gtqgnxnypg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtxtuhpfut.html

[T21] Swift：遍历
来源：http://hz.sysykeji.top/gtlwypjpiu.html

for x in a { print(x) }
来源：http://hz.redwolf501.top/gteavgvdfx.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtvqijuloj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinyuanbaomall.cn/gtmxvoxqwg.html

[T23] Swift：函数
来源：http://hz.sufxvd.cn/gtlaectvbc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xingfuxueyuan.xyz/gtifphwirf.html

[T24] Swift：闭包
来源：http://hz.hnxiangtu.top/gtcauypbfa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtytmflcil.html

[T25] Swift：结构体
来源：http://hz.316326.xyz/gtpgsjzdpw.html

struct P { var x: Int }
来源：http://hz.svipenyu.cn/gtmzrcgjnb.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtfpikuvbx.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtszauohqv.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtfdthbmbu.html

do { try f() } catch { print(error) }
来源：http://hz.mhx1999.top/gtfovqblxk.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtwtgmovjr.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtichohjul.html


<!-- 参考信息 -->