代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtekfvtpbd.html

[R32] 参数个数校验
来源：http://hz.smart0.xyz/gtqsdirgoq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xinyue.icu/gtqccgcefl.html

[R33] 捕获错误并提示行号
来源：http://hz.andypj.xyz/gtqeetvisk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtxsacuebm.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtrvnwvcbh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtvvfhnygq.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gtfaqqhdcy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ywan-chungtsiang.top/gtnsobywoq.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtspceeksh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gtketjzihm.html

[R37] 把输出赋给变量
来源：http://hz.haohaochexian.top/gtaviyvvgf.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gttlgpkppq.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtlqcqeprh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shanyushiyangkeji.top/gtdvfmgixc.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtfaiajdnu.html

cmd > out.log 2>&1
来源：http://hz.ydjk.org.cn/gtunqsowqt.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtejegtbdj.html

echo "log" >> out.log
来源：http://hz.vqdsnc.cn/gtdjqryimx.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtpqgnhbpx.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtwjfltctn.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtqoetjyue.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtzyhpktrb.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtjlsykxuo.html

find . -name "*.log" -type f
来源：http://hz.tanke756.top/gtcgiuczeq.html

[R44] 按修改时间查找
来源：http://hz.gogol.net.cn/gtehsundqg.html

find . -mtime -7 -type f
来源：http://hz.zhixingplan.top/gtssgpqjok.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtblcoysop.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtrnoxyeyi.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtlalpudig.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.kuanghao11.cn/gtjioowrih.html

[R47] sed 单行替换
来源：http://hz.aizwys.cn/gthedpavfx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtygcedffp.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtzgxesozp.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtljyszdhz.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gtoeiwxzcl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtmjjkeidt.html

[R50] awk 求和
来源：http://hz.gzhubu.top/gtxfccridh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtvdccukrk.html

[R51] 排序去重取前几
来源：http://hz.birdmap.top/gtfptyozol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtfawwblef.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtjgkbdilu.html

wc -l a.txt
来源：http://hz.yvedp.cn/gtifxiqhlb.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtlxyizzel.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtyxjbuchd.html

[R54] 比较两个文件
来源：http://hz.jinyuanbaomall.cn/gtekjsvkmf.html

diff a.txt b.txt
来源：http://hz.jinghuilouyu.cn/gtifwmdouy.html

[R55] 压缩与解压
来源：http://hz.pengpengdd.cyou/gtpwrmblbw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtrbmzunvv.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtdnpgwvas.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtthwignra.html

[R57] 远程执行命令
来源：http://hz.zhaomingkeji.xyz/gttxqbpsjp.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtryknvxxs.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtyfbzdbwq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtpmzvmfyw.html

[R59] 发 POST JSON
来源：http://hz.nwbrower.top/gtjdllmzwr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtmyuisxhw.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258.top/gthzdgpwne.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cucudq.cn/gtpiexwgdf.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtvddlcelz.html

df -h;  du -sh *
来源：http://hz.dianchejie.cn/gtmbucxhtl.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gttnoduwht.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtigdyyehj.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gttczwrafw.html

free -h;  ps aux | grep nginx
来源：http://hz.chenzaomai.com/gtwvbxbhst.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtlwfgvazn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtxrvbvdse.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtsiiqqokx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.feifeiyinyue.top/gtjowiyeqf.html

[R66] 定时任务
来源：http://hz.zhongyouzk.top/gtarterlqv.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtghglgyhu.html

[R67] 生成随机十六进制串
来源：http://hz.gotoacloud.top/gtkrxdseam.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtnbxvwvft.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtjaxhbeit.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtjssrmcyf.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtszcdqofh.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtvdeaeixc.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtoyjbyqjl.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtpmnrudfe.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtoefodemu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtynudnfni.html

[R72] 等待端口就绪
来源：http://hz.cashguo.top/gttfaogkxx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtijigbyxh.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtqziaqjuv.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gtwmdrzctd.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtllmkowyb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhiwuduotai.top/gtuostsgvg.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtomzluxun.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtmtcddawa.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtfovkosfp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtytjtjbse.html

[R77] 读取用户输入
来源：http://hz.fengsongda.top/gtjfxwvehu.html

read -rp "请输入: " ans
来源：http://hz.svipenyu.cn/gtylvcfuhe.html

[R78] 交互式菜单
来源：http://hz.zhengqikj.top/gtyopxxanf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtzcpbvtwb.html

[R79] 解析命令行选项
来源：http://hz.wangshuangyany.cn/gtgdsjtzcy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtiekfrsep.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtybrzjepg.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtlinzowrk.html

================================================================================
来源：http://hz.yonumen.top/gtalmgdslv.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gtmfkkqazf.html

================================================================================
来源：http://hz.meibo888.top/gtxfolxrsc.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtgvckwsok.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtgatnexox.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtburmngkk.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtguypjquz.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtxdxmgonx.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtmymagbaq.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gteisaxovv.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gthaqlaxls.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtnuatezjf.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtszwwhhfz.html

strlen(s)
来源：http://hz.nwbrower.top/gtkfjvxvuf.html

[S06] C：字符串比较
来源：http://hz.ydjk.org.cn/gtpfahaxgs.html

strcmp(a, b) == 0
来源：http://hz.0kj1m.cn/gtujnlsktt.html

[S07] C：数组遍历求和
来源：http://hz.cucudq.cn/gtwmagmkbr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhengqikj.top/gticrqicsq.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtcdqssvhq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gtrfcdoznm.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtkdmmjfsh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtcadimkiu.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gttduiijpu.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtjoibksls.html

[S11] C：逐行读文件
来源：http://hz.aizwys.cn/gtfhrrgmbi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtbwwtolcs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtaqzdyets.html

fclose(f);
来源：http://hz.birdmap.top/gtwuieqdnx.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtzwecfaxr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gtkqigapbj.html

[S13] C：宏定义
来源：http://hz.ehwqpu.com/gtyfbqzapy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtvrdmzikd.html

[S14] C：枚举
来源：http://hz.shanyushiyangkeji.top/gtqwzoefhn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtiagellzx.html

[S15] C：类型转换
来源：http://hz.tianlin.xyz/gtmavnrsov.html

(double) a / b
来源：http://hz.zhijiandao.cn/gtzvamdbem.html

[S16] C：位操作置位
来源：http://hz.jiagoushi.top/gtjdkvjgxl.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtcddefbig.html

[S17] C：安全拼接字符串
来源：http://hz.guowangkeji.top/gtpmsqcjlw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yueranfly.top/gtfnpsbnnf.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gttkogthvh.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtmzhlqkfo.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtmcuafgnw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtuxmigjoc.html

[S20] C：二分查找
来源：http://hz.ywan-chungtsiang.top/gtcdsqlpea.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gttyexkmhy.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtupdejdsc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.dianchejie.cn/gtuhwopvle.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtwzpkbxjj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gttenjruew.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtakhdfrzk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangdashe.top/gttyikxnpk.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtlhmbhwtq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tianlin.xyz/gtyghorugd.html

[S25] C：内存拷贝
来源：http://hz.cqqwz.cn/gtcdzcwbtq.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtrwaioani.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtkpnfcefa.html

memset(a, 0, sizeof a);
来源：http://hz.xziqi.cn/gtisavqcas.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtxcmhmjmf.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gthsrawauo.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtczbipvao.html

static int counter = 0;
来源：http://hz.daxiang520.top/gtebfkpyzq.html

[S29] C：变参函数
来源：http://hz.c1oappe.top/gtkmguymzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gttyjvlphf.html

[S30] C：头文件保护
来源：http://hz.xingfuxueyuan.xyz/gtxpebqehi.html

#ifndef X_H
来源：http://hz.quarkkingdee.top/gthxaowqfn.html

#define X_H
来源：http://hz.zhijiandao.cn/gtfusnwedl.html

#endif
来源：http://hz.fzhhl.top/gtctxchvyj.html

[S31] C++：Hello World
来源：http://hz.ywan-chungtsiang.top/gtmjdqximm.html

#include <iostream>
来源：http://hz.xylfe.cn/gtmxistmsr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtfjwdzckz.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtugyontgo.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtmltlvzsx.html

[S33] C++：vector 增删
来源：http://hz.jyoumei.cn/gtejfyffcx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnqzz.top/gtjbocqims.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtuzepzxdk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtjgtjnlfu.html

[S35] C++：map
来源：http://hz.chenlongwang.top/gthvtzysrq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtupqvrawy.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtyaqmuebz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtllqiqrez.html

[S37] C++：set
来源：http://hz.yonumen.top/gtrmlgwkwr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jiagoushi.top/gtodfhghla.html

[S38] C++：排序
来源：http://hz.svipenyu.cn/gtzrhuytqr.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtlqkpvhtr.html

[S39] C++：自定义比较器排序
来源：http://hz.daria6918.cn/gtxdgtfiba.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xinyue.icu/gtwashgocy.html

[S40] C++：查找元素
来源：http://hz.dianchejie.cn/gttzwlfdjz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xinyue.icu/gtsiretaiw.html

[S41] C++：类与构造函数
来源：http://hz.xingfuxueyuan.xyz/gteahgspvu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.feifeiyinyue.top/gtwkfgpdrd.html

[S42] C++：继承与虚函数
来源：http://hz.aibaodan.cn/gtchbmxlhy.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtemdleofg.html

[S43] C++：智能指针
来源：http://hz.xylfe.cn/gtabvymwyd.html

auto p = std::make_unique<int>(5);
来源：http://hz.yvedp.cn/gtbyzdbrqa.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtczhvxgxe.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtlqxpnfjc.html

[S45] C++：lambda
来源：http://hz.yongpay.top/gtcxyaufxp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtsegovncp.html

[S46] C++：函数模板
来源：http://hz.jqgfzy.top/gtdbenltbt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtzkyvbznj.html

[S47] C++：结构化绑定遍历
来源：http://hz.dashuyun.cn/gtrnpwrgnl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sxryk.cn/gtrvtmxgti.html

[S48] C++：逐行读文件
来源：http://hz.daria6918.cn/gtinypwaxe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhaomingkeji.xyz/gttvymnsds.html

while (std::getline(in, line)) { }
来源：http://hz.svipenyu.cn/gtiuleooly.html

[S49] C++：写文件
来源：http://hz.zhongyouzk.top/gtsacapasp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gterbmvifa.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtivorkxdj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gthqyxhorw.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gthjilpjuk.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtlvzqgnav.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtaufjzmaf.html

int size() const noexcept { return n_; }
来源：http://hz.kuanghao11.cn/gthnubtfpq.html

[S53] C++：移动语义
来源：http://hz.daxiang520.top/gtyteolhfy.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gttwltgsjt.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtmedmufwr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pycfn.com/gtervtynaz.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gtjkmxnhts.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtryxvcmue.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtmnmyefti.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gotoacloud.top/gtbbiphrih.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtwbzbaola.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtewlxnxrf.html

[S58] C++：命名空间
来源：http://hz.hysaishi.cn/gtemuqmbia.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gtjwptodrx.html

[S59] C++：静态断言
来源：http://hz.havefunace.top/gtqmslpnzo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtrkmfsvij.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtmqjtobii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gogol.net.cn/gtcuuuyewc.html

================================================================================
来源：http://hz.xziqi.cn/gthqqpxuph.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtyffibzhr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcxandtha.html

[T01] Kotlin：Hello World
来源：http://hz.ydzc1.top/gtqhsabkex.html

println("Hello")
来源：http://hz.cheryme.top/gtedzwkmpg.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gteelzsrri.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtbdlnagvs.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtodtaeicv.html

"值: $b"
来源：http://hz.tianlin.xyz/gtzecmgbxh.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtyvsohiso.html

val n: String? = null;  n?.length
来源：http://hz.nanxinkj.top/gtdijgrved.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtltepvgjl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pycfn.com/gtzmztnkql.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtrxbhlqol.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtfcmanlsg.html

[T07] Kotlin：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtzmsbaivd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtnybfirwd.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gtzplqcrel.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxuanxn.top/gttdvlgbsz.html

[T09] Kotlin：扩展函数
来源：http://hz.xingfuxueyuan.xyz/gtcgawaibt.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtsrjopzfh.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtternzvkg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sweek.top/gttgtwbxfe.html

[T11] Kotlin：协程
来源：http://hz.pengpengdd.cyou/gtrowhaqef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtwxehcjyh.html

[T12] Kotlin：解构声明
来源：http://hz.aizwys.cn/gthwigtbef.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gtehxqgomx.html

[T13] Kotlin：只读 Map
来源：http://hz.tian-w.cn/gtenygvcwl.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtqczoqewn.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtxgqtblyt.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtzjmbomcb.html

[T15] Kotlin：接口
来源：http://hz.pycfn.com/gtyyjmiiom.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtzncaoooc.html

[T16] Swift：Hello World
来源：http://hz.316326.xyz/gtsoqtooph.html

print("Hello")
来源：http://hz.daxiang520.top/gtogtrceli.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtcmobubdq.html

var a = 1;  let b = 2
来源：http://hz.jiagoushi.top/gtiuesfhwu.html

[T18] Swift：字符串插值
来源：http://hz.meibo888.top/gtzrodgley.html

"值: \(b)"
来源：http://hz.sweek.top/gtnjiznqbp.html

[T19] Swift：可选绑定
来源：http://hz.yj202588.top/gtoaztzyla.html

if let n = opt { print(n) }
来源：http://hz.yangfankeji.com/gttoxcttvg.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtpnvqwvhy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtwwrvrrbe.html

[T21] Swift：遍历
来源：http://hz.cqqwz.cn/gtlfxydaiw.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtcdvrycwo.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtxlzqfawt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtmwwbutfh.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtzvcouuoh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhijiandao.cn/gtqvajpflh.html

[T24] Swift：闭包
来源：http://hz.zhijiandao.cn/gtqdirobvp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gtpukilkri.html

[T25] Swift：结构体
来源：http://hz.dianchejie.cn/gtaneozlux.html

struct P { var x: Int }
来源：http://hz.gogol.net.cn/gtctxunulf.html

[T26] Swift：类与重写
来源：http://hz.daxiang520.top/gtgslcqiol.html

class A: Base { override func f() {} }
来源：http://hz.aibaodan.cn/gtnpbxxorl.html

[T27] Swift：错误处理
来源：http://hz.yonumen.top/gttwiegmgb.html

do { try f() } catch { print(error) }
来源：http://hz.hysaishi.cn/gtqdncjyee.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtwkbcvegh.html

enum Color { case red, green }
来源：http://hz.yueranfly.top/gthbwdokuu.html

[T29] Swift：guard 提前返回
来源：http://hz.daria6918.cn/gttbfpifru.html

guard let x = opt else { return }
来源：http://hz.svipenyu.cn/gtgfzrbuug.html

[T30] Swift：协议
来源：http://hz.zhoulong.xyz/gtmsbzwvlu.html

protocol Shape { func area() -> Double }
来源：http://hz.hammf.cn/gteyzbznxa.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtqzonkzrq.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtiqazdhdy.html

[T32] Lua：局部变量
来源：http://hz.kuanghao11.cn/gtxqijgahn.html

local a = 1
来源：http://hz.jinqigufen.top/gtoukxznfx.html

[T33] Lua：表（数组）
来源：http://hz.hongshengwenyu.top/gtkptccntd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nwbrower.top/gtkyrnokle.html

[T34] Lua：遍历表
来源：http://hz.chenlongwang.top/gtberfoqtt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sufxvd.cn/gtmhvlafbu.html


<!-- 参考信息 -->