代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtdejnhpdq.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtpqrhvszy.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtebettglq.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtpfhdibvn.html

echo $((1 + 2 * 3))
来源：http://hz.sysykeji.top/gtvwybloky.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtcwyeuxsp.html

echo "scale=2; 10/3" | bc
来源：http://hz.yanxiufei.cn/gteuakpvww.html

[R29] 定义函数
来源：http://hz.yj202588.top/gtzpfcckfj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtxxbxhnvf.html

[R30] 函数返回状态码
来源：http://hz.zhaomingkeji.xyz/gtoifbapji.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtkpgomwuy.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtmfobzbbg.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gtzsnqovqm.html

[R32] 参数个数校验
来源：http://hz.hysaishi.cn/gtzuyjimcd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtkhilxlhj.html

[R33] 捕获错误并提示行号
来源：http://hz.xziqi.cn/gtkymxiytm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtupapcema.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gtytkhvqaj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtqtegccxa.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gtldshnqag.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydzc1.top/gtygfsyapf.html

[R36] 并发执行多个任务
来源：http://hz.fengsongda.top/gtfagxzxaz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtgqisfcvs.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtxcpedncv.html

files=$(ls -1)
来源：http://hz.zhongyouzk.top/gtqrumzpjg.html

[R38] 管道串联
来源：http://hz.ywan-chungtsiang.top/gtfrkojovk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtutdmcnhh.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtqiimjgqh.html

cmd > out.log 2>&1
来源：http://hz.cqqwz.cn/gtewdbhswt.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gtuqgckxvg.html

echo "log" >> out.log
来源：http://hz.shangyingyoupin.top/gtyidlsguo.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtzvmsbcqq.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gttkoecvgz.html

[R42] 输入重定向
来源：http://hz.zhiwuduotai.top/gtoqbnxleg.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtgzqauxfo.html

[R43] 按名字查找文件
来源：http://hz.hongshengwenyu.top/gtuowpxdbl.html

find . -name "*.log" -type f
来源：http://hz.hnxiangtu.top/gtfrervopk.html

[R44] 按修改时间查找
来源：http://hz.daxiang520.top/gtytztsqvq.html

find . -mtime -7 -type f
来源：http://hz.ydzc1.top/gtvkasdzbf.html

[R45] 批量删除
来源：http://hz.zhongyouzk.top/gtjpkwvrns.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtxkklczpg.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtkhqvitdl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yonumen.top/gtajvizqky.html

[R47] sed 单行替换
来源：http://hz.birdmap.top/gtxnlglhqm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ybcxt.top/gttrirfynt.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtfkdzloww.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtsglpukxp.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtvfvhwjai.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtrzkpoeig.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtstzyudso.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtqspphkon.html

[R51] 排序去重取前几
来源：http://hz.gogol.net.cn/gtrwyjfnrg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtygjmdcxu.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtrhutiktv.html

wc -l a.txt
来源：http://hz.yj20258888.top/gtyoffaxhl.html

[R53] 查看文件头与实时尾
来源：http://hz.zhongyouzk.top/gtdfcxvwzk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtqnzceorb.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtiiuamkbb.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtgyehisqn.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtmqjyuxmd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gzhubu.top/gtufdgkzfl.html

[R56] 远程拷贝
来源：http://hz.guannengcc.top/gtqbqraynj.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtreionnkb.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtqbejakzr.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtmyvbabbj.html

[R58] 下载文件
来源：http://hz.gogol.net.cn/gtvdxszhsh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtxjqrobdy.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtizlqbcpw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtjekbxbwp.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtfrpbnykm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ybcxt.top/gtilhsdggx.html

[R61] 磁盘占用
来源：http://hz.chenzaomai.com/gtwfpselro.html

df -h;  du -sh *
来源：http://hz.guannengcc.top/gtvzenlwsk.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtiourdins.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtkccsnfsy.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtprhcbpjg.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtudhgihzd.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtqzxujmpo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gotoacloud.top/gtodiuheky.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtywzohmup.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shangyingyoupin.top/gtitnzwbqq.html

[R66] 定时任务
来源：http://hz.sufxvd.cn/gtxqwynsdl.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gthgdqvtsl.html

[R67] 生成随机十六进制串
来源：http://hz.fengsongda.top/gtlmzqzite.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtdwmrlzpc.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtvljvvqzb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtdswumddl.html

[R69] 生成随机密码
来源：http://hz.yueranfly.top/gtethaedji.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenzaomai.com/gtpzsrsvks.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtmvwkaovr.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtyzevwemz.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gtrkzwozqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ivvv.top/gtnlkppuws.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtjcsqvnml.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtmorgxgyu.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtthkjrfwt.html

split -l 1000 big.log part_
来源：http://hz.shuidangran.top/gtdzhirfyh.html

[R74] 批量重命名
来源：http://hz.pengpengdd.cyou/gthtatpbnu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtxpnwrrls.html

[R75] 导出环境变量
来源：http://hz.sweek.top/gtuhdioips.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.bjfxy.top/gtlxzlredb.html

[R76] 使用临时文件
来源：http://hz.gzhubu.top/gtymsamhly.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtbnwmsuhi.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtfbzvejod.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gtkxgmzjhp.html

[R78] 交互式菜单
来源：http://hz.chenjidiqi.icu/gtpkqnladm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gotoacloud.top/gtyrlbjwpu.html

[R79] 解析命令行选项
来源：http://hz.sxryk.cn/gtyyrvdkti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gtgpyjrmqu.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gttgsnqqve.html

time ./run.sh
来源：http://hz.ppjwa.cn/gtlpunnbze.html

================================================================================
来源：http://hz.guannengcc.top/gtrfhgsaog.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtmewoygpk.html

================================================================================
来源：http://hz.chenzaomai.com/gtvkuunzct.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtrjukuley.html

#include <stdio.h>
来源：http://hz.pycfn.com/gtwhuqzpwr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.smart0.xyz/gthmudmvid.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gtenbojauv.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtttvyoiwn.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtwtvlhjus.html

int x; scanf("%d", &x);
来源：http://hz.jinqigfzy.top/gtsznlszxl.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtadifovgf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtrqmdzmxq.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gtergncgxj.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtxmtsbiul.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtjhwlmycg.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gttgwkuxyg.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gtreqcuntf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.smart0.xyz/gthtirizxg.html

[S08] C：动态内存分配与释放
来源：http://hz.tanke756.top/gtkcuftszo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gtrdstfgjr.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gtlzcdttqc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtubaardja.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtlkuqnubm.html

int *p = &a;  *p = 5;
来源：http://hz.yuanzhike.top/gtevlsdwab.html

[S11] C：逐行读文件
来源：http://hz.ehwqpu.com/gtyxaauuyq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtfhprbuqs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gtvsoirvyr.html

fclose(f);
来源：http://hz.sxryk.cn/gtacjerbvf.html

[S12] C：写文件
来源：http://hz.ydjk.org.cn/gtlimufgqy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtgkodjkds.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtyfugcjwk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtollecxmp.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtixawtigr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ppjwa.cn/gtckyokiyz.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtghpjxkpl.html

(double) a / b
来源：http://hz.fengsongda.top/gtynzwttdl.html

[S16] C：位操作置位
来源：http://hz.hongshengwenyu.top/gtmihygwkv.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtpuveboyu.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtxxoietoh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtjklnbdqu.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gtnmmxfhcp.html

int main(int argc, char **argv)
来源：http://hz.daxiang520.top/gtbhjrrqfi.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gtjiucwecz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtcmsrkuxe.html

[S20] C：二分查找
来源：http://hz.gzhubu.top/gthgvutdhm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtlemgovbf.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtywpoushv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhoulong.xyz/gtygjurbew.html

[S22] C：字符串转数字
来源：http://hz.tian-w.cn/gtqpkxcyjx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtrxyxevhe.html

[S23] C：随机数
来源：http://hz.guannengcc.top/gtorwcsktz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtxwkyugvp.html

[S24] C：获取本地时间
来源：http://hz.havefunace.top/gtwtdnhqbp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtzrumkxax.html

[S25] C：内存拷贝
来源：http://hz.daxiang520.top/gtoodwdavc.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtaxhvmugz.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtxwtufnil.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtlutcmicv.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtpkcothwf.html

const double PI = 3.14159;
来源：http://hz.cucudq.cn/gtqrbejfpg.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtmebjrqrf.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtalwjbmey.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtaisscfic.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtgfveswbf.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtmbiwosvy.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtypwlxlbi.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtnlmaxrjy.html

#endif
来源：http://hz.aibaodan.cn/gtppftpkgp.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtroawnaox.html

#include <iostream>
来源：http://hz.redwolf501.top/gtiihzsrpp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgufenzy.top/gtvdkrzmqe.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtgldphjdb.html

std::string s = "hi";  s += "!";
来源：http://hz.sysykeji.top/gtbotgfclm.html

[S33] C++：vector 增删
来源：http://hz.zhijiandao.cn/gtjhjwccjb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ppjwa.cn/gtltashzgp.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtsigibmpd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtudqtjmgg.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtyfflsyoq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtdkeynrdo.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtmkighfqr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtktpyzuxt.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtysbjembi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtxzqwhnhu.html

[S38] C++：排序
来源：http://hz.yuanzhike.top/gtvywglezm.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtexzxtncb.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtgntjmocx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yonumen.top/gtbywajtba.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtkegadplk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tanke756.top/gtvipzlnty.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtbzniuaiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gttxinmcwv.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtupylmtqc.html

class B : public Base { public: void f() override {} };
来源：http://hz.xylfe.cn/gtlfqkslhn.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtxrokfsqo.html

auto p = std::make_unique<int>(5);
来源：http://hz.sweek.top/gtxcmoqlcg.html

[S44] C++：引用传参
来源：http://hz.jqgfzy.top/gtancyztxd.html

void inc(int &x) { ++x; }
来源：http://hz.aibaodan.cn/gtsnssvywx.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtyeefbjcr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jiagoushi.top/gtgjmlcfer.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtberaqlmw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gtfabwotaa.html

[S47] C++：结构化绑定遍历
来源：http://hz.316326.xyz/gtqpheeggy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtqqpihhby.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtjcpiwycw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgufenzy.top/gtlkkxygxr.html

while (std::getline(in, line)) { }
来源：http://hz.zhengqikj.top/gtvwbjmhvz.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtcehcynbx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtxkfascrj.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtjcedrroi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtbtgybbae.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtkamspvgy.html

static_cast<double>(a) / b
来源：http://hz.xuanzx.com/gtpxkkquad.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtndqgwife.html

int size() const noexcept { return n_; }
来源：http://hz.redwolf501.top/gtwyujgovt.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtjacwwonj.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtlrnitfif.html

[S54] C++：异常处理
来源：http://hz.fengsongda.top/gtjakebymo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xingfuxueyuan.xyz/gtufdvopby.html

[S55] C++：结构化绑定
来源：http://hz.gaohongyu789.top/gtwstipoeh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gtiomldhys.html

[S56] C++：optional
来源：http://hz.jiagoushi.top/gtzabhkdkv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinqigfzy.top/gtqzmhywix.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtqnzhyqus.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtrigslcmq.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtvdnnxvbj.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhaomingkeji.xyz/gtqopcrbvt.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gtewicdyli.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtkubxrtxg.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtmwhbrsya.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtbqdpoyjs.html

================================================================================
来源：http://hz.sweek.top/gtbjptwjup.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtljlmmgsz.html

================================================================================
来源：http://hz.yvedp.cn/gtgjknyeod.html

[T01] Kotlin：Hello World
来源：http://hz.ywan-chungtsiang.top/gtlnywortx.html

println("Hello")
来源：http://hz.pycfn.com/gtdutykbpf.html

[T02] Kotlin：变量
来源：http://hz.fengsongda.top/gtgdpgnwoj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gtwtilfnue.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtydamikza.html

"值: $b"
来源：http://hz.gzhubu.top/gtjexffnsw.html

[T04] Kotlin：空安全
来源：http://hz.gogol.net.cn/gtpcimkprl.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtdsvsoltb.html

[T05] Kotlin：when 表达式
来源：http://hz.nwbrower.top/gtwgdfvfui.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtycrsctwz.html

[T06] Kotlin：集合映射
来源：http://hz.gotoacloud.top/gtexfkpfqf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenlongwang.top/gtsfchqexe.html

[T07] Kotlin：集合过滤
来源：http://hz.yuxming.cn/gtwojjoioi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtfgplicjy.html

[T08] Kotlin：数据类
来源：http://hz.jiagoushi.top/gtccowqfat.html

data class User(val name: String, val age: Int)
来源：http://hz.mhx1999.top/gtvzucdtvq.html

[T09] Kotlin：扩展函数
来源：http://hz.cdnleiting.top/gttyjfefyb.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtevrxvcdl.html

[T10] Kotlin：默认参数
来源：http://hz.svipenyu.cn/gtvcirlebr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jyoumei.cn/gtpfnmslzl.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtzplinrdq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigufen.top/gtlzycdxlx.html

[T12] Kotlin：解构声明
来源：http://hz.xinyue.icu/gtxdvhyids.html

val (a, b) = Pair(1, 2)
来源：http://hz.jianghu66.top/gtelwrgofw.html

[T13] Kotlin：只读 Map
来源：http://hz.zdqjudy.top/gttkuswlhp.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtlbqjitdw.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtbozbvfot.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtlkgnicjn.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtezweajtf.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtpzivcxqu.html

[T16] Swift：Hello World
来源：http://hz.hysaishi.cn/gtgztjwwwb.html

print("Hello")
来源：http://hz.gotoacloud.top/gttkdfsseu.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtzlgrbpxm.html

var a = 1;  let b = 2
来源：http://hz.redwolf501.top/gttgsuvmog.html

[T18] Swift：字符串插值
来源：http://hz.sxryk.cn/gtvumxnnpg.html

"值: \(b)"
来源：http://hz.guowangkeji.top/gtvkjflunj.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gtchcfrtvr.html

if let n = opt { print(n) }
来源：http://hz.iojbl.cn/gtpeaxftmc.html

[T20] Swift：数组操作
来源：http://hz.hongshengwenyu.top/gtjgjdrjwp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.redwolf501.top/gtdqwrjzpt.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtklvlxnpb.html

for x in a { print(x) }
来源：http://hz.zycfv.cn/gtqirnhsje.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtxgflxtpq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gtetgwrexs.html

[T23] Swift：函数
来源：http://hz.shzxlz.cn/gtuvkvgerm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tanke756.top/gtqzlnonxs.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtavimfsyx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.andypj.xyz/gtpxkjmwzo.html

[T25] Swift：结构体
来源：http://hz.jinqigfzy.top/gtamlpnuqz.html

struct P { var x: Int }
来源：http://hz.snrcjt.cn/gtyzfklbcw.html

[T26] Swift：类与重写
来源：http://hz.hnxiangtu.top/gtckgbveuj.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtwjrcmkuo.html

[T27] Swift：错误处理
来源：http://hz.zhoulong.xyz/gtyxntkqjk.html

do { try f() } catch { print(error) }
来源：http://hz.0kj1m.cn/gtaenziecf.html

[T28] Swift：枚举
来源：http://hz.haohaochexian.top/gtvylgslag.html

enum Color { case red, green }
来源：http://hz.fzhhl.top/gtgmvivssg.html


<!-- 参考信息 -->