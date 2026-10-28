代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.mhx1999.top/gtsxsvuvrw.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtcjlaamqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtdjhasxlj.html

[R33] 捕获错误并提示行号
来源：http://hz.jlsjyb.cn/gtionotalw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtuvuudxkl.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gthpqtuwco.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtypphgjbr.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtgsclamrk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtzulvlocl.html

[R36] 并发执行多个任务
来源：http://hz.sysykeji.top/gtoepkvtkq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gthcemvqyq.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtmogqfyxn.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtetaczpsc.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtknzrbpyj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sufxvd.cn/gtupsjcwzb.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gtezhabqsa.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtolsikdop.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gtzkvmwvba.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gthakalqke.html

[R41] 丢弃输出
来源：http://hz.zhaomingkeji.xyz/gttpvmasfx.html

cmd >/dev/null 2>&1
来源：http://hz.bjfxy.top/gtyzldpmlq.html

[R42] 输入重定向
来源：http://hz.jiagoushi.top/gtgwoekkhi.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtsphljsme.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtvlxjihui.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtnecovwjn.html

[R44] 按修改时间查找
来源：http://hz.316326.xyz/gtrqlxddgo.html

find . -mtime -7 -type f
来源：http://hz.mhx1999.top/gtrapaexob.html

[R45] 批量删除
来源：http://hz.meibo888.top/gtuwcyraqz.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtwxphwfin.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtvztqfqka.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtufdvhpgr.html

[R47] sed 单行替换
来源：http://hz.shangyingyoupin.top/gtepdcqhzm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gtttlacsmd.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtfkjtpwlo.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangshuangyany.cn/gteqmwssng.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtrkximvpn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtldjdzghr.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtipnwkqjb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtkdmbyxpn.html

[R51] 排序去重取前几
来源：http://hz.shangyingyoupin.top/gtrsgixnxc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daxiang520.top/gtclplawwi.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtpmmknmvy.html

wc -l a.txt
来源：http://hz.tian-w.cn/gtrkyawrxu.html

[R53] 查看文件头与实时尾
来源：http://hz.chenzaomai.com/gtbtbzrwpd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tianlin.xyz/gtgltuoxrw.html

[R54] 比较两个文件
来源：http://hz.jinghuilouyu.cn/gtzbpciqnq.html

diff a.txt b.txt
来源：http://hz.yuxming.cn/gtkorycqma.html

[R55] 压缩与解压
来源：http://hz.daria6918.cn/gteqiclepo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gtmewthmxw.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtcdgsoxya.html

scp file user@host:/path/
来源：http://hz.zhiwuduotai.top/gtgvqlvyik.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtibbauhkg.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtbmavuzjz.html

[R58] 下载文件
来源：http://hz.guowangkeji.top/gtkhcnhuub.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gtgunxruok.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtrglzieqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gtfcagfjxx.html

[R60] 只看 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtzreundvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gtjawrifdk.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtzyufousy.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtyytmnowo.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtsvhequdt.html

du -ah . | sort -rh | head -10
来源：http://hz.zhongyouzk.top/gtovxtthlr.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtsjebuxcy.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtnzxrylxv.html

[R64] 结束进程
来源：http://hz.wangshuangyany.cn/gtbeaujpwu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtodaujngm.html

[R65] 查看端口占用
来源：http://hz.shuidangran.top/gtrvgrlwuo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gtwqlzwqgi.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtovjidfay.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtykpvayiq.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtntwqurbc.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gthgxzmbkx.html

[R68] 计算文件校验值
来源：http://hz.haohaochexian.top/gtidwjyuda.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtldadrjog.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtonxiyqvd.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtcnglrttq.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtrsxcuzvr.html

date +%s;  date -d @1700000000
来源：http://hz.yongpay.top/gtjqrnuznu.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtklnbopjp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtmydggmsa.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtacpvqtgb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gtjrzoghnx.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtmksadfjg.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtfrbzedve.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtgvhsvrxf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.kuanghao11.cn/gtyeywkuaw.html

[R75] 导出环境变量
来源：http://hz.xuanzx.com/gtuywrooqy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtpfgokkro.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtrtzmcwaz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtppavxaki.html

[R77] 读取用户输入
来源：http://hz.svipenyu.cn/gtwkvaroao.html

read -rp "请输入: " ans
来源：http://hz.sxryk.cn/gtqgjheesl.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtexeiggea.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shzxlz.cn/gtubtlbjgo.html

[R79] 解析命令行选项
来源：http://hz.yanxiufei.cn/gtysaltzhl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj20258.top/gtjgigihio.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtvseunqyx.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtuhxyauvk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrqpjiplj.html

S. C / C++ 专题
来源：http://hz.bjfxy.top/gtswjqznhq.html

================================================================================
来源：http://hz.zdqjudy.top/gtcwiwukvt.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtkfyfpuij.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gticebynvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fengsongda.top/gtduzzkhru.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtafsafzcp.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtdpqhtwcs.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtbmgcicpc.html

int x; scanf("%d", &x);
来源：http://hz.fengsongda.top/gtvqulgdvu.html

[S04] C：字符串复制
来源：http://hz.ehwqpu.com/gthvrmfswm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.feifeiyinyue.top/gtzbbzycup.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtryrulwyu.html

strlen(s)
来源：http://hz.hysaishi.cn/gtcxbiverd.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtpsvjyjdp.html

strcmp(a, b) == 0
来源：http://hz.shuidangran.top/gtvcugzzdp.html

[S07] C：数组遍历求和
来源：http://hz.xziqi.cn/gtsnklpcvg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gaohongyu789.top/gtszclprfx.html

[S08] C：动态内存分配与释放
来源：http://hz.wangshuangyany.cn/gtuojwfijs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ehwqpu.com/gtmtqktfwj.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtidfzrjhr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtqunfgmki.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtnmgwcpxe.html

int *p = &a;  *p = 5;
来源：http://hz.hongshengwenyu.top/gthqiujwtz.html

[S11] C：逐行读文件
来源：http://hz.jqgfzy.top/gtxwpxnwbk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.kuanghao11.cn/gtbnxauclw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuanzx.com/gttsozwlzv.html

fclose(f);
来源：http://hz.nanxinkj.top/gtcjqovwtc.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtqzyafsyc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtxxkwpuvd.html

[S13] C：宏定义
来源：http://hz.iojbl.cn/gtvtooafdc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yueranfly.top/gtlclkfynd.html

[S14] C：枚举
来源：http://hz.zycfv.cn/gtzwtcrtzg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtpjkkpgzt.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtsflzsvsi.html

(double) a / b
来源：http://hz.jianghu66.top/gtbzxgmkzv.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtcgfuxvej.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gttclngehn.html

[S17] C：安全拼接字符串
来源：http://hz.xuetiantiany.cn/gtshhxgifu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gtjjqqkgdn.html

[S18] C：命令行参数
来源：http://hz.xziqi.cn/gtvdlkhugh.html

int main(int argc, char **argv)
来源：http://hz.yangfankeji.com/gtgrfmtgyq.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtkyrspemi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtjlbhcgnz.html

[S20] C：二分查找
来源：http://hz.birdmap.top/gtxponbsnz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtfjjkzrzl.html

[S21] C：字符类别判断
来源：http://hz.sysykeji.top/gtagaqbczz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtyukkybbd.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtveeyqdmi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtbralsxhx.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtkutqtfmv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gtosvnelza.html

[S24] C：获取本地时间
来源：http://hz.zhiwuduotai.top/gtdbbjpdwo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhengqikj.top/gtkbghwpys.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtedghdjmz.html

memcpy(dst, src, n);
来源：http://hz.zhaomingkeji.xyz/gtftwdlruc.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtmwqerxbw.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtotccwkju.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtbpqqqazg.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtzzemaqkq.html

[S28] C：静态变量
来源：http://hz.ppjwa.cn/gttocwokpr.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gtemnrkngs.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtybuhldmn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xinyue.icu/gtxeaqbbbk.html

[S30] C：头文件保护
来源：http://hz.gogol.net.cn/gtuxzrbtur.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtjhjdyzfi.html

#define X_H
来源：http://hz.nanxuanxn.top/gtkptfkqmh.html

#endif
来源：http://hz.yj20258.top/gtcumhezvr.html

[S31] C++：Hello World
来源：http://hz.yangfankeji.com/gtdwnxrhzs.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gtilspgowe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtejuhgcqz.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtemmqanay.html

std::string s = "hi";  s += "!";
来源：http://hz.tanke756.top/gtbzokmawp.html

[S33] C++：vector 增删
来源：http://hz.jinqigufen.top/gtofcxzhgi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhongyouzk.top/gtalgrjnap.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtwyhjgrpa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tianlin.xyz/gtxxavgywv.html

[S35] C++：map
来源：http://hz.pengpengdd.cyou/gtxetpmmjc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtdhmgtnqo.html

[S36] C++：unordered_map
来源：http://hz.nanxuanxn.top/gtclfnjijy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtxizyeiba.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtvvvcibez.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.haohaochexian.top/gtsukhjuwd.html

[S38] C++：排序
来源：http://hz.yuanzhike.top/gtoylpbesh.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtludapiov.html

[S39] C++：自定义比较器排序
来源：http://hz.haohaochexian.top/gtmqifwgxm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtrvovsvze.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtkqtlhrfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtfzbhmtub.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gtqxxyhvgr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtsbkumkst.html

[S42] C++：继承与虚函数
来源：http://hz.daria6918.cn/gttezzsgww.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigufen.top/gtytddvpjw.html

[S43] C++：智能指针
来源：http://hz.feifeiyinyue.top/gtieqgyklh.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gttmxcimxv.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtezmwdxma.html

void inc(int &x) { ++x; }
来源：http://hz.xuanzx.com/gtumrsjzak.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtwpspkzzx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fengsongda.top/gtyymqyswo.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtpliggzjh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtslxjdvlh.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtjsuriamh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtbwiilktl.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtpaxulfkh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtyqhlsrxc.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtvlnacyzv.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtfaryfozt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gthgvqggkq.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtjosucdam.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gtdkmoxbqu.html

[S51] C++：显式类型转换
来源：http://hz.jyoumei.cn/gtuqqijvkc.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtadieobpq.html

[S52] C++：const 与 noexcept
来源：http://hz.zhijiandao.cn/gtbfqaniey.html

int size() const noexcept { return n_; }
来源：http://hz.xuanzx.com/gtkznoytql.html

[S53] C++：移动语义
来源：http://hz.xinyue.icu/gtfvjdbbvx.html

std::vector<int> w = std::move(v);
来源：http://hz.ydzc1.top/gttvblvydu.html

[S54] C++：异常处理
来源：http://hz.zhoulong.xyz/gtoyjeooyo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtxgztysrs.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtmqdvpvib.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtkkskdjqb.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtiqevvldd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtxrtybbmp.html

[S57] C++：编译期常量
来源：http://hz.yvedp.cn/gtdugendmn.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtnqgeqyar.html

[S58] C++：命名空间
来源：http://hz.cdnleiting.top/gtcadwbsre.html

namespace ns { int f() { return 1; } }
来源：http://hz.hfpthk.cn/gtkojcsjea.html

[S59] C++：静态断言
来源：http://hz.zhoulong.xyz/gtfgcrkaka.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gtuilpobpw.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtpzlaqqsx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtqpxagbyl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjyvedgvp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtmiddcpdk.html

================================================================================
来源：http://hz.xziqi.cn/gtmbgiiagr.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtrqhlfyxs.html

println("Hello")
来源：http://hz.chenlongwang.top/gtdkmhbdiw.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtmgwjrfad.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtaoyexgpj.html

[T03] Kotlin：字符串模板
来源：http://hz.ppjwa.cn/gttjpfmfew.html

"值: $b"
来源：http://hz.chenzaomai.com/gtxnhnqqws.html

[T04] Kotlin：空安全
来源：http://hz.xinyue.icu/gtoonawalz.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtknjusxoy.html

[T05] Kotlin：when 表达式
来源：http://hz.316326.xyz/gtnqvuxila.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtcatjfjse.html

[T06] Kotlin：集合映射
来源：http://hz.hfpthk.cn/gtpekyjsox.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.9152youxi.cn/gtiikfqmzc.html

[T07] Kotlin：集合过滤
来源：http://hz.yj202588.top/gtydnvmatd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gthjenzzmj.html

[T08] Kotlin：数据类
来源：http://hz.hywenlv.cn/gtopfcdjnt.html

data class User(val name: String, val age: Int)
来源：http://hz.wangshuangyany.cn/gtaicdwwdl.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtclvfdxpr.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258888.top/gtldrssnpx.html

[T10] Kotlin：默认参数
来源：http://hz.shuidangran.top/gttjlvqbqy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cqqwz.cn/gtnvvyynmw.html

[T11] Kotlin：协程
来源：http://hz.meibo888.top/gtqvugulai.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.bjfxy.top/gtkypsgjjj.html

[T12] Kotlin：解构声明
来源：http://hz.ydjk.org.cn/gtifjlervm.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gtcxxityqs.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtzmkbhopk.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtuutfturx.html

[T14] Kotlin：循环
来源：http://hz.zdqjudy.top/gtcmwhawkc.html

for (i in 1..10) println(i)
来源：http://hz.feifeiyinyue.top/gtajciogot.html

[T15] Kotlin：接口
来源：http://hz.zhixingplan.top/gtzzoxanwh.html

interface Shape { fun area(): Double }
来源：http://hz.ybcxt.top/gtdxyqdfei.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gtnyigxbov.html

print("Hello")
来源：http://hz.316326.xyz/gtlcqjzhvz.html

[T17] Swift：变量与常量
来源：http://hz.tianlin.xyz/gtxmnqmqwa.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gtxzyeydxh.html

[T18] Swift：字符串插值
来源：http://hz.sxryk.cn/gtfgucxibf.html

"值: \(b)"
来源：http://hz.yangfankeji.com/gtqxeizvnc.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtfcbopmzt.html

if let n = opt { print(n) }
来源：http://hz.svipenyu.cn/gtrtikabmi.html

[T20] Swift：数组操作
来源：http://hz.hongshengwenyu.top/gtmmpktjdm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtgfyovlfd.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtqbktbxti.html

for x in a { print(x) }
来源：http://hz.xinyue.icu/gtsbojniuv.html

[T22] Swift：字典
来源：http://hz.hysaishi.cn/gtttuotoek.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.316326.xyz/gtqongwoid.html

[T23] Swift：函数
来源：http://hz.shzxlz.cn/gtylqnetin.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gaohongyu789.top/gtqpirares.html

[T24] Swift：闭包
来源：http://hz.feifeiyinyue.top/gtnmkfwfia.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gthklicdab.html

[T25] Swift：结构体
来源：http://hz.c1oappe.top/gthckrlvve.html

struct P { var x: Int }
来源：http://hz.sufxvd.cn/gtntidnvlb.html

[T26] Swift：类与重写
来源：http://hz.feifeiyinyue.top/gtnubpaffz.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangkeji.top/gtvkydgsgn.html

[T27] Swift：错误处理
来源：http://hz.jiagoushi.top/gtnmwvgotq.html

do { try f() } catch { print(error) }
来源：http://hz.jinyuanbaomall.cn/gtzfnfanpf.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangtech.top/gtbjqscegw.html

enum Color { case red, green }
来源：http://hz.snrcjt.cn/gtbtlijjzu.html

[T29] Swift：guard 提前返回
来源：http://hz.zhaomingkeji.xyz/gtykdrckqa.html

guard let x = opt else { return }
来源：http://hz.jinqigfzy.top/gtswghcojp.html

[T30] Swift：协议
来源：http://hz.ybcxt.top/gtrnjcjgcy.html

protocol Shape { func area() -> Double }
来源：http://hz.xylfe.cn/gtjnksotvt.html

[T31] Lua：Hello World
来源：http://hz.hammf.cn/gtqqpehrrx.html

print("Hello")
来源：http://hz.yongpay.top/gtahyjnhve.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtaphzanzp.html

local a = 1
来源：http://hz.sxryk.cn/gthpihbyca.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtiwvsfziu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sufxvd.cn/gttwilarbu.html

[T34] Lua：遍历表
来源：http://hz.gaohongyu789.top/gtiypffuoq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yanxiufei.cn/gtpgbdhhyu.html


<!-- 参考信息 -->