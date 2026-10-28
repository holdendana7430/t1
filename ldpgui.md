代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxuanxn.top/gtowmvqtev.html

[R26] 命令替换
来源：http://hz.ehwqpu.com/gtlyqaooup.html

now=$(date +%F); echo "$now"
来源：http://hz.birdmap.top/gtfnrjwdgg.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtbylujzza.html

echo $((1 + 2 * 3))
来源：http://hz.aizwys.cn/gtifklluqu.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtkrpoprpy.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtucysqdsf.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtkaxbynqx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gttiqkgpkw.html

[R30] 函数返回状态码
来源：http://hz.yuanzhike.top/gtapafdevb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gtfwyxginu.html

[R31] 局部变量
来源：http://hz.tianlin.xyz/gtqaltfopq.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydzc1.top/gtenovxocb.html

[R32] 参数个数校验
来源：http://hz.yonumen.top/gtevsjouxn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gttsyeymep.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gtmyvdtbxw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtffxotycw.html

[R34] 退出时清理
来源：http://hz.nanxuanxn.top/gtvkeveber.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtngguydvr.html

[R35] 后台执行并等待
来源：http://hz.jqgufenzy.top/gtyeojdifz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtfxpskkak.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtwngccmgc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sufxvd.cn/gtlfqytpwd.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gteoydhfvd.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtyuhxibzv.html

[R38] 管道串联
来源：http://hz.gaohongyu789.top/gtrlgcjeqz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guowangkeji.top/gtzmbyhfbp.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtlrqoltgl.html

cmd > out.log 2>&1
来源：http://hz.yj20258.top/gtaxtsgbpq.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtvquldqzc.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtbvcnzsxn.html

[R41] 丢弃输出
来源：http://hz.zhongyouzk.top/gtcizndpcr.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gttjuvrcgd.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gtutwvdnmq.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gtykbrehkv.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtucegwljw.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtnotrgkda.html

[R44] 按修改时间查找
来源：http://hz.guowangkeji.top/gtdvwwawgr.html

find . -mtime -7 -type f
来源：http://hz.xuetiantiany.cn/gtmdhifrvv.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gtholmnnef.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtmsshwivr.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtghyswvcv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xziqi.cn/gtjzuazbmt.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtxobqborg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtvtebqrfa.html

[R48] awk 取指定列
来源：http://hz.guannengcc.top/gtwouzbfsb.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenlongwang.top/gtdaaxuweg.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtlwriqjdc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtealecauf.html

[R50] awk 求和
来源：http://hz.ybcxt.top/gtgjflkzjz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtfqpvjnwr.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtobqxlgue.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.feifeiyinyue.top/gtdzzcslfa.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gtikynsdkk.html

wc -l a.txt
来源：http://hz.fengsongda.top/gttfpouoao.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtmanecsuh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtptdmnzux.html

[R54] 比较两个文件
来源：http://hz.cashguo.top/gtqrqfdxpv.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtfgvwqrxo.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gthazcjxbp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangtech.top/gtkbvuaawv.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangtech.top/gthdsyuaif.html

scp file user@host:/path/
来源：http://hz.aizwys.cn/gtabhgquoi.html

[R57] 远程执行命令
来源：http://hz.gaohongyu789.top/gtkddkzxzl.html

ssh user@host 'uptime'
来源：http://hz.birdmap.top/gtwylmtgji.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtkuvqsage.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtphdkziob.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtmpozwrmx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tianlin.xyz/gtqccwavsk.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtqpkmuzmo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sufxvd.cn/gtfdmfjqqv.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtdpshjguk.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtpxsmpbek.html

[R62] 找最占空间的文件
来源：http://hz.yangfankeji.com/gtedvirctd.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtfykdezxa.html

[R63] 内存与进程
来源：http://hz.sweek.top/gtxihhtjlf.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtebscekcg.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtqtfnzpto.html

kill -9 $(pgrep -f app.py)
来源：http://hz.snrcjt.cn/gtmmxxamgd.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gthnfsfjfk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gtsqucozrs.html

[R66] 定时任务
来源：http://hz.svipenyu.cn/gtzjtsdiiz.html

crontab -e;  crontab -l
来源：http://hz.ehwqpu.com/gtwbswquut.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtrggdtioz.html

openssl rand -hex 16
来源：http://hz.gaohongyu789.top/gttsezjjof.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtoasfnsxr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtizycwbye.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtxxgrvnmn.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangshuangyany.cn/gtrsdzuags.html

[R70] 时间戳与互转
来源：http://hz.tanke756.top/gtdzfgojhq.html

date +%s;  date -d @1700000000
来源：http://hz.xinyue.icu/gtypslrmrh.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtvwayipaz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtuqiqqkvs.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtynwcuiis.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtbsansfmi.html

[R73] 分割大日志
来源：http://hz.9152youxi.cn/gteabpbuxa.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtbjovqbos.html

[R74] 批量重命名
来源：http://hz.zhiwuduotai.top/gtkoheikpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ywan-chungtsiang.top/gtanrbztxm.html

[R75] 导出环境变量
来源：http://hz.fzhhl.top/gtprawahpq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj202588.top/gtakmhibnc.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtkxfeahwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtzxhywlnf.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtylofaqks.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gthboaxmzi.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtikitzlod.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cucudq.cn/gtbaugnypa.html

[R79] 解析命令行选项
来源：http://hz.yanxiufei.cn/gtunoxyrgf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhijiandao.cn/gtrazgghmw.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gtcbfopbht.html

time ./run.sh
来源：http://hz.zhongyouzk.top/gtimvadyup.html

================================================================================
来源：http://hz.jianghu66.top/gtywbibkmf.html

S. C / C++ 专题
来源：http://hz.yuanzhike.top/gtmhhpnzyp.html

================================================================================
来源：http://hz.hfpthk.cn/gtkdcvejgs.html

[S01] C：Hello World
来源：http://hz.redwolf501.top/gtniimtheq.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtirrmtckl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuanzhike.top/gtkvuvqdfy.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtopgcunas.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtmhoypvtu.html

[S03] C：读入整数
来源：http://hz.yuanzhike.top/gtkmnpdsmr.html

int x; scanf("%d", &x);
来源：http://hz.cashguo.top/gtchueuglv.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtkyexkndx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hammf.cn/gtzbpkitvj.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtzrlnmgtb.html

strlen(s)
来源：http://hz.quarkkingdee.top/gthqjmpjte.html

[S06] C：字符串比较
来源：http://hz.cqqwz.cn/gtjqqqtndj.html

strcmp(a, b) == 0
来源：http://hz.shzxlz.cn/gtjhmvxlfo.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gthlsvyztq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gthzswqsaq.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtcqbhvvoy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dashuyun.cn/gtndxnstnx.html

[S09] C：结构体定义与初始化
来源：http://hz.mhx1999.top/gtkibxygyq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtszhhbaba.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtcaraywtf.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtnnrkeloz.html

[S11] C：逐行读文件
来源：http://hz.cqqwz.cn/gtdrhqarka.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtbpnliwlv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jlsjyb.cn/gtctbqtqfq.html

fclose(f);
来源：http://hz.yvedp.cn/gtuzstesyi.html

[S12] C：写文件
来源：http://hz.zycfv.cn/gtjlhrmjdo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cucudq.cn/gtitkuxant.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gtuojsocky.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gtvvlqwhqc.html

[S14] C：枚举
来源：http://hz.jinqigfzy.top/gtouvqsgsj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gtotxahvgl.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtazatdpwi.html

(double) a / b
来源：http://hz.wangdashe.top/gtxkzkpsqr.html

[S16] C：位操作置位
来源：http://hz.xziqi.cn/gtazfkarpx.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtyirpmhij.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtdbuqeeom.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtusciyxfn.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtnzphcwuy.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gthfciplwr.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gtfuhheipx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtrnogxzht.html

[S20] C：二分查找
来源：http://hz.chenzaomai.com/gtimercafe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtbokgmhqr.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gttnzsndqs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuxming.cn/gtupdfkdhq.html

[S22] C：字符串转数字
来源：http://hz.dashuyun.cn/gtjkuzmmfj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtsrigrwvn.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gtazuxqnrc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtnjrfsecr.html

[S24] C：获取本地时间
来源：http://hz.c1oappe.top/gtkkkqmfcj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtalrzovoe.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtoklvoczk.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtpzptocpv.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtqfplchkc.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtnvggdlmk.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtifrorred.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtiseujxzr.html

[S28] C：静态变量
来源：http://hz.shanyushiyangtech.top/gthpfpmedh.html

static int counter = 0;
来源：http://hz.fzhhl.top/gtwkkedxjy.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtolyudczh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hywenlv.cn/gtiolpeizm.html

[S30] C：头文件保护
来源：http://hz.daxiang520.top/gtmilfpnsh.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtexwnyzjm.html

#define X_H
来源：http://hz.ydjk.org.cn/gtcnnvqjsq.html

#endif
来源：http://hz.cashguo.top/gtxeksisml.html

[S31] C++：Hello World
来源：http://hz.wangdashe.top/gtpdcromsc.html

#include <iostream>
来源：http://hz.zycfv.cn/gtxaunympf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtkfvtmkxc.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtghloxicz.html

std::string s = "hi";  s += "!";
来源：http://hz.tianlin.xyz/gtoybrsqon.html

[S33] C++：vector 增删
来源：http://hz.daria6918.cn/gtwmsgweiz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtlrzchuis.html

[S34] C++：遍历 vector
来源：http://hz.hywenlv.cn/gtnikjcmwy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zdqjudy.top/gteanbxgoi.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtxcczaikj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gthkzugsjr.html

[S36] C++：unordered_map
来源：http://hz.gaohongyu789.top/gtztcuyyvt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gttommjecf.html

[S37] C++：set
来源：http://hz.redwolf501.top/gtcyiznasn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtnxyvxbkn.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtprhgujwr.html

std::sort(v.begin(), v.end());
来源：http://hz.chenzaomai.com/gtwqcxhnpw.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtpgjiduwb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtfnuzlpiy.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gthkxpgixe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhongyouzk.top/gtatvdbkej.html

[S41] C++：类与构造函数
来源：http://hz.jiagoushi.top/gtyzkvicqr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenzaomai.com/gtjgtfgrem.html

[S42] C++：继承与虚函数
来源：http://hz.shzxlz.cn/gtxkrgkcmu.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenjidiqi.icu/gtbymwlptk.html

[S43] C++：智能指针
来源：http://hz.gogol.net.cn/gtchzmbzln.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gturhvfksn.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtfytcclxn.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtjtjvukwk.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtnhkcjjdl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cqqwz.cn/gtclyjxbjv.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtrcwkqlkh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtkurndsew.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxinkj.top/gteawvfckx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtqlyxnyrn.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtwftjuxha.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtvoldurug.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gttovjgptr.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtdhsnncbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhengqikj.top/gtdjgffaha.html

[S50] C++：格式化数字
来源：http://hz.yangfankeji.com/gtrvmhaimm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtxwhuvjnr.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gtnaytassl.html

static_cast<double>(a) / b
来源：http://hz.0kj1m.cn/gtsqymbqit.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtzzwomgqw.html

int size() const noexcept { return n_; }
来源：http://hz.hnxiangtu.top/gtkaxmtlod.html

[S53] C++：移动语义
来源：http://hz.mhx1999.top/gtpcwwurlo.html

std::vector<int> w = std::move(v);
来源：http://hz.cucudq.cn/gtisccycss.html

[S54] C++：异常处理
来源：http://hz.aibaodan.cn/gtuuqabtds.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gtngkbuxup.html

[S55] C++：结构化绑定
来源：http://hz.0kj1m.cn/gtkviqrces.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtwthtroth.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtyfqtrcnb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtaqfacden.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtzdlkyiry.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtyjhbthvp.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangtech.top/gtolqoxunb.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gtxtfuduja.html

[S59] C++：静态断言
来源：http://hz.yueranfly.top/gtmnyyjtwv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtcmnmujoc.html

[S60] C++：遍历并删除元素
来源：http://hz.hfpthk.cn/gtgahdrnsh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gtfyfpbyyl.html

================================================================================
来源：http://hz.ydzc1.top/gtwwfigehh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtbomxgzte.html

================================================================================
来源：http://hz.ivvv.top/gtvaruauws.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gtzphapbcl.html

println("Hello")
来源：http://hz.316326.xyz/gtnnsajmwl.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtgljuwizr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtalgjjklc.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtwrekrzds.html

"值: $b"
来源：http://hz.hammf.cn/gtrtbrlank.html

[T04] Kotlin：空安全
来源：http://hz.jinqigufen.top/gtrylxaqdp.html

val n: String? = null;  n?.length
来源：http://hz.9152youxi.cn/gtxlwtuoxn.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtwowcefmn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gotoacloud.top/gtktbvhkol.html

[T06] Kotlin：集合映射
来源：http://hz.xylfe.cn/gtlrtjowym.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtrenhiklb.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtnbzcztzn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtwrmosmcs.html

[T08] Kotlin：数据类
来源：http://hz.daria6918.cn/gtwplbsijw.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtrxvhfqfi.html

[T09] Kotlin：扩展函数
来源：http://hz.pengpengdd.cyou/gtqyadsbzf.html

fun String.exclaim() = this + "!"
来源：http://hz.snrcjt.cn/gtzflbeinp.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtsforwtdq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtbuhuwnmr.html

[T11] Kotlin：协程
来源：http://hz.ydjk.org.cn/gtlzuaayso.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cheryme.top/gtlspuqxiu.html

[T12] Kotlin：解构声明
来源：http://hz.aizwys.cn/gtdyjaorpy.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtxjtgmqgs.html

[T13] Kotlin：只读 Map
来源：http://hz.redwolf501.top/gtbjrdhhra.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtylqbxmgs.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtkvmpytgy.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtgsrdtfnt.html

[T15] Kotlin：接口
来源：http://hz.0kj1m.cn/gtanoctytu.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gtknjipllj.html

[T16] Swift：Hello World
来源：http://hz.hywenlv.cn/gtjlrxqzvr.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtvhqsloxk.html

[T17] Swift：变量与常量
来源：http://hz.gotoacloud.top/gtkaxoengp.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gtpgyufhbf.html

[T18] Swift：字符串插值
来源：http://hz.52xcode.cn/gtcqbsbrma.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtvfzsrtmu.html

[T19] Swift：可选绑定
来源：http://hz.smart0.xyz/gtfvrrzwjn.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gtvyoijzel.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gtmpplqxux.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtqhhbffif.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtvbbyhnnn.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtaulbtlvp.html

[T22] Swift：字典
来源：http://hz.zhongyouzk.top/gtvhcwzgve.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gteeepxmqw.html

[T23] Swift：函数
来源：http://hz.hywenlv.cn/gthiutadpd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtnjuvcskc.html

[T24] Swift：闭包
来源：http://hz.jianghu66.top/gtudddhqye.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtndpnptmu.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gturhnbugo.html

struct P { var x: Int }
来源：http://hz.nwbrower.top/gtbqxxfzzu.html

[T26] Swift：类与重写
来源：http://hz.c1oappe.top/gtzntgdokm.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtnlttlhio.html

[T27] Swift：错误处理
来源：http://hz.ppjwa.cn/gtyfhpfcxj.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtvwdfwhtg.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtuyikcpyx.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gttxkgmzwn.html


<!-- 参考信息 -->