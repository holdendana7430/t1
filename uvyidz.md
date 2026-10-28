代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gttyrzewvy.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtldewzylt.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtdvnqtdkt.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtoumpdvfv.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtgvkuwdga.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtbkcyjzxg.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtlragamga.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtpseklcam.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.vqdsnc.cn/gtvzszexlx.html

[R30] 函数返回状态码
来源：http://hz.chenlongwang.top/gtbysdputm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtkrdmtmtb.html

[R31] 局部变量
来源：http://hz.bjfxy.top/gtmmukbgih.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtsdfdcrkm.html

[R32] 参数个数校验
来源：http://hz.ivvv.top/gtyjalenpy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtvbropwoa.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtjfefbich.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtfxvtuolh.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtntnbevla.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gthzpyfvpv.html

[R35] 后台执行并等待
来源：http://hz.zhijiandao.cn/gtztqorhzi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zycfv.cn/gtcagcgzbf.html

[R36] 并发执行多个任务
来源：http://hz.jinqigfzy.top/gtwkjdikix.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gtplraqgax.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtteaemwal.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtqdnayrcm.html

[R38] 管道串联
来源：http://hz.wangshuangyany.cn/gtbxgnnrxv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tian-w.cn/gtagclgfnd.html

[R39] 重定向标准输出与错误
来源：http://hz.quarkkingdee.top/gtnfjlykjs.html

cmd > out.log 2>&1
来源：http://hz.fengsongda.top/gtiqqgecce.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtjcjovarb.html

echo "log" >> out.log
来源：http://hz.0kj1m.cn/gtxkhzkwyv.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtdqopgong.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gttyxcryns.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gthliiwsod.html

wc -l < a.txt
来源：http://hz.zhijiandao.cn/gtbkmcvqis.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtptosbhpc.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtyjbakksr.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gtcacbaubi.html

find . -mtime -7 -type f
来源：http://hz.hammf.cn/gtljmtiyab.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gtstubsbel.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtjyldgurw.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtgtzxwttk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhengqikj.top/gtttkwjcja.html

[R47] sed 单行替换
来源：http://hz.nwbrower.top/gtebvhhmvr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtjsdyaknl.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtssjpoehz.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtfcjymbzw.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtfejbjkbu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnqzz.top/gtmojjyrcv.html

[R50] awk 求和
来源：http://hz.quarkkingdee.top/gtsgrkkpnc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtrkzwbejk.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtjuixtslv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtmqgjjkui.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtfcdzdicv.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtsjkfywbr.html

[R53] 查看文件头与实时尾
来源：http://hz.shzxlz.cn/gtfsoadmrb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258.top/gtvivdqjwq.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtdpzyqurx.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtegnxragp.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtmmodpgbx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangtech.top/gtpkowgkwk.html

[R56] 远程拷贝
来源：http://hz.hysaishi.cn/gtrwgllbub.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtdxwyedcu.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtwupdpdgj.html

ssh user@host 'uptime'
来源：http://hz.yonumen.top/gtdsskmllr.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtzpxbiuck.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnqzz.top/gtjmzysugo.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtnkudagaw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gterpgolxn.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gtrrudqqzu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.snrcjt.cn/gtxojxscpr.html

[R61] 磁盘占用
来源：http://hz.daria6918.cn/gtnacimkzu.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gttvukbhrm.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtiooubuzm.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtnzsvyemr.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtylmndrky.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtmvwjnltl.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtuzmdffgu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtyxrhqlor.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtutszzwnm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gtuuaacwsm.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gthrppjylh.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtzpxwzgbp.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtaoqrripa.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtkzkyoomc.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtelbrbdkq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtqzkuqluz.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtsulvxflz.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtkfvkxmse.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtliswfhpn.html

date +%s;  date -d @1700000000
来源：http://hz.jyoumei.cn/gtdogjbqql.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtlnnzxsmz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gtijgdoriz.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtkoydcbts.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daria6918.cn/gtpwrdkirp.html

[R73] 分割大日志
来源：http://hz.hongshengwenyu.top/gtlatmxaqt.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtwrzjjmay.html

[R74] 批量重命名
来源：http://hz.zhiwuduotai.top/gtlendaqsu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xinyue.icu/gtqqvhehoj.html

[R75] 导出环境变量
来源：http://hz.dashuyun.cn/gtqdlqgcqc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ybcxt.top/gtlriobqwq.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gttrmvrsfa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtqgvxuklo.html

[R77] 读取用户输入
来源：http://hz.pengpengdd.cyou/gtnahnnkyi.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtvcepheqe.html

[R78] 交互式菜单
来源：http://hz.zhengqikj.top/gttswtyazj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gtwdkwedqk.html

[R79] 解析命令行选项
来源：http://hz.gotoacloud.top/gtzrbfgeft.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtkiqmiasl.html

[R80] 查看脚本执行耗时
来源：http://hz.shzxlz.cn/gtrlwynxsn.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtrkrtkugn.html

================================================================================
来源：http://hz.cucudq.cn/gteobkvvah.html

S. C / C++ 专题
来源：http://hz.smart0.xyz/gtxfrhyfob.html

================================================================================
来源：http://hz.cashguo.top/gttuuoohuo.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtxlzuczmx.html

#include <stdio.h>
来源：http://hz.sweek.top/gtfjburupq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yanxiufei.cn/gtoupeakkf.html

[S02] C：变量与格式化输出
来源：http://hz.cashguo.top/gtrggjawem.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtfxohbwnm.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gthbvydfkb.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtrtzkiyik.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtrlzhdrbz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtvfvgkcxw.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gtzzbmqoww.html

strlen(s)
来源：http://hz.tian-w.cn/gtxjfdppii.html

[S06] C：字符串比较
来源：http://hz.fengsongda.top/gtsuiddpsv.html

strcmp(a, b) == 0
来源：http://hz.daria6918.cn/gttlfsahzk.html

[S07] C：数组遍历求和
来源：http://hz.smart0.xyz/gtslcsxfvt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.snrcjt.cn/gtvcgctttq.html

[S08] C：动态内存分配与释放
来源：http://hz.jinghuilouyu.cn/gtjattvyam.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yongpay.top/gtltqbycoh.html

[S09] C：结构体定义与初始化
来源：http://hz.tianlin.xyz/gtzskfqlqu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gtcmiwabua.html

[S10] C：指针与解引用
来源：http://hz.haohaochexian.top/gtlohhshjg.html

int *p = &a;  *p = 5;
来源：http://hz.zhiwuduotai.top/gtbnivgzvo.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtuyubvxsc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhengqikj.top/gtszejzzhl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtvvdlntve.html

fclose(f);
来源：http://hz.nanxuanxn.top/gtdwjmrlei.html

[S12] C：写文件
来源：http://hz.tian-w.cn/gtluwonvjv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj202588.top/gtgffeszti.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtxtcvgjlv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gtuxdmjfcz.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtvhixjzzx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj202588.top/gtjurhpqtm.html

[S15] C：类型转换
来源：http://hz.cashguo.top/gtqkghvfho.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gthutnpyrj.html

[S16] C：位操作置位
来源：http://hz.shangyingyoupin.top/gtcxjyvjtd.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gtbonwohbg.html

[S17] C：安全拼接字符串
来源：http://hz.jyoumei.cn/gtnhcbunjo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gtafdtaafw.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtzoveuayx.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtzruqkvgj.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtntderkja.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gthxgebmbe.html

[S20] C：二分查找
来源：http://hz.kuanghao11.cn/gtmkbiawgr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtophmgkpj.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtgxexxkau.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aibaodan.cn/gtsuoxqgtx.html

[S22] C：字符串转数字
来源：http://hz.andypj.xyz/gtinhjadze.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinyuanbaomall.cn/gtkgxqkuqv.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtrmltghoj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.andypj.xyz/gtrmfqefni.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gtbacfwzyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhaomingkeji.xyz/gtiahgywlc.html

[S25] C：内存拷贝
来源：http://hz.9152youxi.cn/gtbmuooehk.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtrtnkpwhk.html

[S26] C：内存清零
来源：http://hz.pycfn.com/gtdgfcdmtg.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtbzbmnkhr.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gtzagrhplw.html

const double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtetyxntbv.html

[S28] C：静态变量
来源：http://hz.svipenyu.cn/gtepozqina.html

static int counter = 0;
来源：http://hz.chenjidiqi.icu/gtgwlntjqg.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtjgyxjgpv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shzxlz.cn/gttilwkksp.html

[S30] C：头文件保护
来源：http://hz.pycfn.com/gtzxuzpqht.html

#ifndef X_H
来源：http://hz.daria6918.cn/gtdptpnkjy.html

#define X_H
来源：http://hz.cqqwz.cn/gtnvbreorw.html

#endif
来源：http://hz.yangfankeji.com/gtsqyodoix.html

[S31] C++：Hello World
来源：http://hz.xuetiantiany.cn/gtddpjcftp.html

#include <iostream>
来源：http://hz.ydzc1.top/gtubbvetcq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gtkefssncm.html

[S32] C++：字符串
来源：http://hz.quarkkingdee.top/gtyfeezqxc.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtvkfycplu.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gtqonfqjqa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gteitivwwk.html

[S34] C++：遍历 vector
来源：http://hz.fzhhl.top/gtscinbcyw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gtxvxcuswk.html

[S35] C++：map
来源：http://hz.shuidangran.top/gtmgvmmduf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gthecremca.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtnkuftxak.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gthpsitqrx.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtjfjruxmj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.bjfxy.top/gtqgqklkta.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtgbzqkrio.html

std::sort(v.begin(), v.end());
来源：http://hz.wangshuangyany.cn/gtmjhljwnl.html

[S39] C++：自定义比较器排序
来源：http://hz.cheryme.top/gtihkxgofd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ehwqpu.com/gtsdqmvgcy.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtbjpgakrs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtsxrtivuv.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtkqvoagwi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cucudq.cn/gtgifcgvlk.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtpqbbppso.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtcvnbrfsi.html

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtafcbylsc.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtxwacjnfc.html

[S44] C++：引用传参
来源：http://hz.yanxiufei.cn/gtapsqeyto.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtfvkjjsno.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtiouvescv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtimhhprxh.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtpaspkxov.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cashguo.top/gtvacldhpi.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuanzhike.top/gttamokvoa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgfzy.top/gtaflvsmtq.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gttqswprpl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtfqybwkaz.html

while (std::getline(in, line)) { }
来源：http://hz.quarkkingdee.top/gtrjxmcgjx.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtozfvvtny.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtmunmgcvt.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtwnhqxrxb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aizwys.cn/gthupydwdb.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gtyoxympfv.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtndcnfpnh.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtdpupkzua.html

int size() const noexcept { return n_; }
来源：http://hz.zhiwuduotai.top/gtkdzhqhmt.html

[S53] C++：移动语义
来源：http://hz.pengpengdd.cyou/gtqgyayebn.html

std::vector<int> w = std::move(v);
来源：http://hz.zhengqikj.top/gtujeudrnj.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtisabqmgn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydzc1.top/gthqhrlnyn.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtkdpoxfsn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtfqmyfmlj.html

[S56] C++：optional
来源：http://hz.shzxlz.cn/gtlfioepqy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtpoedfeng.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtggemosuo.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtjflxchzn.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gteoyjjewz.html

namespace ns { int f() { return 1; } }
来源：http://hz.ppjwa.cn/gtmdgpvvqj.html

[S59] C++：静态断言
来源：http://hz.jinyuanbaomall.cn/gtqurkhzcs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtafrqqvvk.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtsglzygaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtbijsllbv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbercsure.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ppjwa.cn/gtlbcxtmkx.html

================================================================================
来源：http://hz.ybcxt.top/gtmtlsrpur.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtiaearqqy.html

println("Hello")
来源：http://hz.xylfe.cn/gtdbrmtawr.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtwfflqqmm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtkmocqint.html

[T03] Kotlin：字符串模板
来源：http://hz.cheryme.top/gtuzytpwbi.html

"值: $b"
来源：http://hz.gotoacloud.top/gtlflqoxah.html

[T04] Kotlin：空安全
来源：http://hz.sufxvd.cn/gtqcchcnvz.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtszkprgcs.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gteblyqnga.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shuidangran.top/gtyeluvbkx.html

[T06] Kotlin：集合映射
来源：http://hz.jyoumei.cn/gtfhudzflc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tanke756.top/gtylqncwpa.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtfmqrzzmx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fengsongda.top/gtusvrzeti.html

[T08] Kotlin：数据类
来源：http://hz.aizwys.cn/gthjuwjbie.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtuatkljxl.html

[T09] Kotlin：扩展函数
来源：http://hz.dianchejie.cn/gthotzccjb.html

fun String.exclaim() = this + "!"
来源：http://hz.fengsongda.top/gtmildncak.html

[T10] Kotlin：默认参数
来源：http://hz.zhoulong.xyz/gtstqcazir.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ywan-chungtsiang.top/gtryrcoxto.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtuhhiaoxc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtvaegkrva.html

[T12] Kotlin：解构声明
来源：http://hz.zycfv.cn/gtdvsygspx.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtkmjqvyyi.html

[T13] Kotlin：只读 Map
来源：http://hz.yongpay.top/gtomsnbpqr.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gtfuffdeyj.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtoaoorycy.html

for (i in 1..10) println(i)
来源：http://hz.nanxinkj.top/gtlbdhrbrk.html

[T15] Kotlin：接口
来源：http://hz.bjfxy.top/gtkscjfhdv.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gthtrdsmpr.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gtevhlvkwg.html

print("Hello")
来源：http://hz.iojbl.cn/gtqhkujjrp.html

[T17] Swift：变量与常量
来源：http://hz.redwolf501.top/gtmtybqswj.html

var a = 1;  let b = 2
来源：http://hz.xinyue.icu/gtooeipjve.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtuscjfsav.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gtrdcfzsvz.html

[T19] Swift：可选绑定
来源：http://hz.ivvv.top/gtainfirdh.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtkzkeftpi.html

[T20] Swift：数组操作
来源：http://hz.gotoacloud.top/gtrubrjnez.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yonumen.top/gtzixvnfzq.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtmyixbqhr.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtrhrgcyly.html

[T22] Swift：字典
来源：http://hz.52xcode.cn/gteswoymcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtcgnqthzk.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gthvvolzbe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sxryk.cn/gtuxywyhqm.html

[T24] Swift：闭包
来源：http://hz.ehwqpu.com/gtrmuaoycp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.52xcode.cn/gtmxtywbtm.html

[T25] Swift：结构体
来源：http://hz.havefunace.top/gtwcgqoiyt.html

struct P { var x: Int }
来源：http://hz.hysaishi.cn/gtncnlitef.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gthmtedsia.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtyjpoyoxq.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gtsmyjpdym.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtlbimhxhq.html

[T28] Swift：枚举
来源：http://hz.xylfe.cn/gtjmjkaceh.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtgvsjkkzo.html


<!-- 参考信息 -->