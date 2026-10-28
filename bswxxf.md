代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtunbzewvt.html

[R24] 大小写转换
来源：http://hz.xylfe.cn/gtkegftiux.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pengpengdd.cyou/gtbhrbcibx.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtwtubgvpp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtislughqn.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtdmstxvfc.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtwtbrgeeq.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtnwjruohz.html

echo $((1 + 2 * 3))
来源：http://hz.guannengcc.top/gtzgpvaurp.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gthdclyaqj.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtjnjtatif.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtkvicrrzw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtjcxwwexm.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gttovkbkam.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dashuyun.cn/gteweblazd.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gtnosqpcud.html

f() { local x=1; echo "$x"; }
来源：http://hz.quarkkingdee.top/gtypbmhywo.html

[R32] 参数个数校验
来源：http://hz.birdmap.top/gttdztbbxb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtwlxvqwss.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtdvcxqpvk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenjidiqi.icu/gtofwwxgko.html

[R34] 退出时清理
来源：http://hz.pengpengdd.cyou/gtdbtexxyu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gtdbnesbms.html

[R35] 后台执行并等待
来源：http://hz.chenjidiqi.icu/gthqirhbgs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtnfmtfsoj.html

[R36] 并发执行多个任务
来源：http://hz.yangfankeji.com/gtwumyzaco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ybcxt.top/gtscdcmlre.html

[R37] 把输出赋给变量
来源：http://hz.ydjk.org.cn/gtoppxvuhw.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtjruoeeto.html

[R38] 管道串联
来源：http://hz.hammf.cn/gtkrsxdoko.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtugmzutsv.html

[R39] 重定向标准输出与错误
来源：http://hz.gzhubu.top/gtqoiyvytx.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtjyetssmq.html

[R40] 追加写日志
来源：http://hz.cashguo.top/gtdtjrwagr.html

echo "log" >> out.log
来源：http://hz.xuanzx.com/gtujjywlvu.html

[R41] 丢弃输出
来源：http://hz.dianchejie.cn/gtjyjzyzog.html

cmd >/dev/null 2>&1
来源：http://hz.jyoumei.cn/gtgepbuedq.html

[R42] 输入重定向
来源：http://hz.zhoulong.xyz/gtdhudsgbe.html

wc -l < a.txt
来源：http://hz.yonumen.top/gtwldubryo.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtslbwxtgd.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtllsyjlgf.html

[R44] 按修改时间查找
来源：http://hz.aizwys.cn/gtmdfmpndi.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtbulpamkj.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gtvqzxxpoh.html

find . -name "*.tmp" -delete
来源：http://hz.xylfe.cn/gtzrxmvdsb.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gtsyzyjcaw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtfnktimqs.html

[R47] sed 单行替换
来源：http://hz.pycfn.com/gtxvsyfebe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shangyingyoupin.top/gtyzupbnsg.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtlhcslnxw.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtilugjtab.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtoluzygxy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtjcusdedk.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtrvopzwzr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.mhx1999.top/gtjlabqfgb.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtpjhovebw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuetiantiany.cn/gtadwkmktp.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtthvamobk.html

wc -l a.txt
来源：http://hz.tian-w.cn/gtqerogdpp.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtrvkgjzxo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cucudq.cn/gtfngxonkg.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtycszciaz.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtotmiohgm.html

[R55] 压缩与解压
来源：http://hz.hywenlv.cn/gtqlihiqbk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtmydvezbk.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtwkwriksc.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtwuwwdkkv.html

[R57] 远程执行命令
来源：http://hz.hnqzz.top/gtoeyppjvx.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gtsfddqdci.html

[R58] 下载文件
来源：http://hz.cdnleiting.top/gtrmbqvhqt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtptqhoneu.html

[R59] 发 POST JSON
来源：http://hz.hfpthk.cn/gtvjihnbac.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gttbckukkd.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtisomnxeo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtfbnmvhkb.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gteazqfaaq.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtgpohxwrs.html

[R62] 找最占空间的文件
来源：http://hz.zycfv.cn/gtlawdqrpj.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgfzy.top/gtuyomohzg.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gtolyzwxlo.html

free -h;  ps aux | grep nginx
来源：http://hz.yongpay.top/gtfjukvdjc.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtjjngajyi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtfpjtbuae.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtfrfeljil.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258888.top/gtlxmbthvw.html

[R66] 定时任务
来源：http://hz.nwbrower.top/gtkhhqhsfb.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtrkmjkshf.html

[R67] 生成随机十六进制串
来源：http://hz.daria6918.cn/gtczuqhwnr.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gthqldrpff.html

[R68] 计算文件校验值
来源：http://hz.cqqwz.cn/gtvwqojtpj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtffbqccpc.html

[R69] 生成随机密码
来源：http://hz.nwbrower.top/gttuwkkmvt.html

head -c 16 /dev/urandom | base64
来源：http://hz.vqdsnc.cn/gtzwtteduj.html

[R70] 时间戳与互转
来源：http://hz.tanke756.top/gtgtlkirxp.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gtfkfdxlvg.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gtafvoqmzt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinghuilouyu.cn/gtqkjeyoif.html

[R72] 等待端口就绪
来源：http://hz.xuanzx.com/gtyomhqkuf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.snrcjt.cn/gtuopmfstj.html

[R73] 分割大日志
来源：http://hz.yuanzhike.top/gtoqbxwsxs.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtjuumswsg.html

[R74] 批量重命名
来源：http://hz.zhiwuduotai.top/gtfldweteh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtifnroaao.html

[R75] 导出环境变量
来源：http://hz.jinqigufen.top/gtabtimzwi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuanzx.com/gtsbolrgxw.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtqgqztvpo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtbypbsamw.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtkuoaclyi.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtjksgnznv.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gtackcltyk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtwspyayop.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtulwefazb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtkqxntcay.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtixhqpkws.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtsuutorrk.html

================================================================================
来源：http://hz.daxiang520.top/gtxuhcvljy.html

S. C / C++ 专题
来源：http://hz.yueranfly.top/gtikibfeou.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtestwchsu.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtxjieiwax.html

#include <stdio.h>
来源：http://hz.dashuyun.cn/gtgzrwthlb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtkixddmlo.html

[S02] C：变量与格式化输出
来源：http://hz.sxryk.cn/gtqudabaoq.html

int a = 10; printf("%d\n", a);
来源：http://hz.sweek.top/gtnkdsippd.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtobasyzpn.html

int x; scanf("%d", &x);
来源：http://hz.jqgufenzy.top/gtbqojtpkv.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtkqltpify.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cucudq.cn/gtxchzsizn.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gtdzoawxfb.html

strlen(s)
来源：http://hz.redwolf501.top/gtvkxguyzz.html

[S06] C：字符串比较
来源：http://hz.52xcode.cn/gtmqdhbugo.html

strcmp(a, b) == 0
来源：http://hz.smart0.xyz/gtsfowfrft.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gthubhssvp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtdnlusfzb.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtcbqrtqbv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gtvilxvuqs.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtsgtquqzr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj202588.top/gtaolamdbm.html

[S10] C：指针与解引用
来源：http://hz.yangfankeji.com/gtnahhkwxr.html

int *p = &a;  *p = 5;
来源：http://hz.hammf.cn/gtnickgzpm.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtrbzpkjxn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtppwsopfx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yongpay.top/gtmhfiuatn.html

fclose(f);
来源：http://hz.shzxlz.cn/gtxwftarzo.html

[S12] C：写文件
来源：http://hz.gotoacloud.top/gthhqzbwwb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gtykmulkyc.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtowdeqtnf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gtggamaqel.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtqxkevjbi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangshuangyany.cn/gtbuuhhdwt.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtjbzhyreh.html

(double) a / b
来源：http://hz.fengsongda.top/gtvopwoyqr.html

[S16] C：位操作置位
来源：http://hz.xziqi.cn/gtrfeytorf.html

x |= (1 << 3);
来源：http://hz.0kj1m.cn/gtctajdxud.html

[S17] C：安全拼接字符串
来源：http://hz.cheryme.top/gtdttuphqx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yangfankeji.com/gtphsuiedy.html

[S18] C：命令行参数
来源：http://hz.yj20258888.top/gtlffrhizb.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtewpfqjmn.html

[S19] C：快速排序
来源：http://hz.chenzaomai.com/gtyerywude.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtjhjynywg.html

[S20] C：二分查找
来源：http://hz.jqgfzy.top/gtseibguhz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtbsiqmxlw.html

[S21] C：字符类别判断
来源：http://hz.yonumen.top/gtzokvzmwk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.0kj1m.cn/gtcvemfedn.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtdsqovdim.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhengqikj.top/gttiebhsly.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtcotsejie.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtqntrxtaj.html

[S24] C：获取本地时间
来源：http://hz.ehwqpu.com/gtwdqpwxmo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtmmizzujh.html

[S25] C：内存拷贝
来源：http://hz.gzhubu.top/gtbpqvlume.html

memcpy(dst, src, n);
来源：http://hz.gzhubu.top/gthbysphlv.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gtamtxbyjd.html

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gtqwmjdwou.html

[S27] C：定义常量
来源：http://hz.ivvv.top/gtpttpljlr.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtxjpvvavx.html

[S28] C：静态变量
来源：http://hz.guowangkeji.top/gtxrleizxs.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtqryqboua.html

[S29] C：变参函数
来源：http://hz.zhaomingkeji.xyz/gtkbttkahf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aibaodan.cn/gtlqrtsunz.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtfrybiirf.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtmmhqcyie.html

#define X_H
来源：http://hz.zhongyouzk.top/gtbfnzaafk.html

#endif
来源：http://hz.jinqigufen.top/gtsgqinzxg.html

[S31] C++：Hello World
来源：http://hz.zhengqikj.top/gtodvxbwtn.html

#include <iostream>
来源：http://hz.yuanzhike.top/gthcwgflxk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gtmmxlgqct.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtanolpalf.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtgrokngru.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtjzeyduuv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtfujdblse.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtdadnlasi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtsrhdkysh.html

[S35] C++：map
来源：http://hz.aizwys.cn/gtgagkzfas.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtmdktcphr.html

[S36] C++：unordered_map
来源：http://hz.guowangkeji.top/gtqonahifw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gteysrfjxu.html

[S37] C++：set
来源：http://hz.yvedp.cn/gtnzlxuhxq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ivvv.top/gtppskgivw.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtbwsqaxpm.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtckfgdzdo.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gttuooqggk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jianghu66.top/gtffxjbuzs.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtwpckhror.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yvedp.cn/gtymiuegls.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtuyagovca.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtcbkzfhei.html

[S42] C++：继承与虚函数
来源：http://hz.daria6918.cn/gtdzueeekw.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtnsmcbnfi.html

[S43] C++：智能指针
来源：http://hz.iojbl.cn/gtkcoocrwy.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gtujbedfpy.html

[S44] C++：引用传参
来源：http://hz.zycfv.cn/gtpgzvgmjr.html

void inc(int &x) { ++x; }
来源：http://hz.ydzc1.top/gtjyasstyu.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtkhkzopte.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.52xcode.cn/gtoxhbuoqf.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtolkcrngf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtdxpyzmvt.html

[S47] C++：结构化绑定遍历
来源：http://hz.nwbrower.top/gtiweaixoz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydzc1.top/gtuqyndxfp.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gtizqjfegb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtxxppwpav.html

while (std::getline(in, line)) { }
来源：http://hz.0kj1m.cn/gtlhaawaox.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtjnqawuec.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtkjtfydxk.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtnbsygqbh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtxkrkgyye.html

[S51] C++：显式类型转换
来源：http://hz.zhixingplan.top/gtcgtfkiat.html

static_cast<double>(a) / b
来源：http://hz.yuanzhike.top/gtsqvssibe.html

[S52] C++：const 与 noexcept
来源：http://hz.guowangkeji.top/gtzfqiwhmc.html

int size() const noexcept { return n_; }
来源：http://hz.guannengcc.top/gtvgwqymvd.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtnkrcquvn.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangkeji.top/gtmuvdggfs.html

[S54] C++：异常处理
来源：http://hz.gogol.net.cn/gtroqcagls.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gttblldout.html

[S55] C++：结构化绑定
来源：http://hz.tianlin.xyz/gtlrayrgbv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtvvcjdpng.html

[S56] C++：optional
来源：http://hz.wangdashe.top/gtwgiatknq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.redwolf501.top/gtkbriwngw.html

[S57] C++：编译期常量
来源：http://hz.9152youxi.cn/gttvjsmlia.html

constexpr int N = 10;
来源：http://hz.sweek.top/gtwyknihzd.html

[S58] C++：命名空间
来源：http://hz.zhaomingkeji.xyz/gtbiyslvqu.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gtlamzyquv.html

[S59] C++：静态断言
来源：http://hz.sufxvd.cn/gtyoivgglo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtngpkjwtc.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gtnczcdxgb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuanzx.com/gtcaxvnlex.html

================================================================================
来源：http://hz.iojbl.cn/gtgmypsbto.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtvvnkcrfr.html

================================================================================
来源：http://hz.tanke756.top/gtbozruhkw.html

[T01] Kotlin：Hello World
来源：http://hz.dashuyun.cn/gtmvkaadry.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtthjciqge.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtpnpafqrx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtekevtoan.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtvnzgroma.html

"值: $b"
来源：http://hz.yvedp.cn/gtjdmofllz.html

[T04] Kotlin：空安全
来源：http://hz.zhaomingkeji.xyz/gtenvcxaes.html

val n: String? = null;  n?.length
来源：http://hz.zhijiandao.cn/gttjwpqzsz.html

[T05] Kotlin：when 表达式
来源：http://hz.yongpay.top/gtzqcbuulg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtwujyilrx.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtgjknthkv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtpooqulrq.html

[T07] Kotlin：集合过滤
来源：http://hz.chenlongwang.top/gtbhdsprdd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtjjclmrhf.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtkczxuhaa.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtbhergruv.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtzapcbmgc.html

fun String.exclaim() = this + "!"
来源：http://hz.chenjidiqi.icu/gtfwtxmphi.html

[T10] Kotlin：默认参数
来源：http://hz.ydjk.org.cn/gtdgvjriva.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtyjjaxavk.html

[T11] Kotlin：协程
来源：http://hz.sufxvd.cn/gteppvoubd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuanzhike.top/gtmclarifr.html

[T12] Kotlin：解构声明
来源：http://hz.aibaodan.cn/gtdmrqdudu.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gtniayrbhy.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtgprokbgu.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gtywoczfdp.html

[T14] Kotlin：循环
来源：http://hz.zycfv.cn/gtgtkzijee.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtlvzxnppu.html

[T15] Kotlin：接口
来源：http://hz.guannengcc.top/gtyzfvbnep.html

interface Shape { fun area(): Double }
来源：http://hz.jiagoushi.top/gttbdzokxe.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtypqazkar.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtvnxrbjeo.html

[T17] Swift：变量与常量
来源：http://hz.hnxiangtu.top/gtcndxzmxy.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtinhjzvgg.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtkumslicz.html

"值: \(b)"
来源：http://hz.cashguo.top/gthslvsomf.html

[T19] Swift：可选绑定
来源：http://hz.guannengcc.top/gtyuvtuyjw.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtbhvbgomw.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtpetgomrg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtwmcxcqbz.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtcaspfyom.html

for x in a { print(x) }
来源：http://hz.yueranfly.top/gtlffwjznf.html

[T22] Swift：字典
来源：http://hz.yueranfly.top/gtoanxiujg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gthvdwsbyv.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtlohcvpfs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtrmmppcor.html

[T24] Swift：闭包
来源：http://hz.yj20258888.top/gtngzxlksq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nwbrower.top/gtewpuvhwm.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtgluvrnbc.html

struct P { var x: Int }
来源：http://hz.sysykeji.top/gtqobbjjwy.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtgfwzagqz.html

class A: Base { override func f() {} }
来源：http://hz.chenzaomai.com/gtucfiozhv.html


<!-- 参考信息 -->