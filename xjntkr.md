代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zycfv.cn/gtkulzyylk.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtuchoiovp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jianghu66.top/gtwccuphek.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtcojuokwo.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtvznnqraa.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtugxatrpp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtsoqolxvt.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gtosxrrily.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtzocvjktw.html

[R22] 截取子串
来源：http://hz.wangdashe.top/gtnplrltuu.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtfbfnqlii.html

[R23] 字符串替换
来源：http://hz.hysaishi.cn/gtfsfakiqj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtuarharce.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtuflxzdcf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtuogpmcmz.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gttjaiuwns.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtdebxanil.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtvrmmzwuo.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtilmrcxli.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtaemfuoea.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtyhfnhito.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtdftrazfa.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtwciwodpr.html

[R29] 定义函数
来源：http://hz.mhx1999.top/gttqkqsbyt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtjkcwnhng.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtbyosmgfy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtsbhztpfr.html

[R31] 局部变量
来源：http://hz.ywan-chungtsiang.top/gtbuyqrjqs.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtrierdjsx.html

[R32] 参数个数校验
来源：http://hz.jqgfzy.top/gtqabvjxxs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.smart0.xyz/gtpzbpwlgb.html

[R33] 捕获错误并提示行号
来源：http://hz.aizwys.cn/gtijewcyql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtgxtirfdh.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtcyucwtyz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtwdhzxrgi.html

[R35] 后台执行并等待
来源：http://hz.zhixingplan.top/gtuawjsead.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gthlurfato.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtgjqqucgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gttzjarggp.html

[R37] 把输出赋给变量
来源：http://hz.gaohongyu789.top/gtxzjfdaqh.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtuzargvfz.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtmasxbvzf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cqqwz.cn/gtagxmxblc.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtqhdasvob.html

cmd > out.log 2>&1
来源：http://hz.gotoacloud.top/gtiypbtmfc.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtfjptgode.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gtnxilthex.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtentlofdn.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtpjegligh.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtotebmpyy.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtykppkcpw.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtqylmcwnw.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtfkwxnuiw.html

[R44] 按修改时间查找
来源：http://hz.316326.xyz/gtdvsgqulu.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtaiwautgc.html

[R45] 批量删除
来源：http://hz.tianlin.xyz/gtiiamwdfu.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtqkamvrtr.html

[R46] 递归替换文件内容
来源：http://hz.zhixingplan.top/gtdgrhqshs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtfrkpwmpz.html

[R47] sed 单行替换
来源：http://hz.cheryme.top/gtgiynyuyz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuanzx.com/gtqixdjnvj.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtsggvdiki.html

awk '{print $1, $3}' a.txt
来源：http://hz.havefunace.top/gtqccnspuj.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtumukwokt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtxlhleewl.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtfbqgwizd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtxbvnajbk.html

[R51] 排序去重取前几
来源：http://hz.svipenyu.cn/gtpcyiktwi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guannengcc.top/gtpwszoeoj.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtlljhezwo.html

wc -l a.txt
来源：http://hz.shzxlz.cn/gtfgedmavv.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtstjqnynf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuetiantiany.cn/gteytmxtnw.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtpdsevjml.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtuuszufhe.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtjyapmius.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtcotcclke.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtamhvztad.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtgkbvabzg.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtuumshded.html

ssh user@host 'uptime'
来源：http://hz.zhaomingkeji.xyz/gtcenrlqzn.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtqlqvnlwl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ehwqpu.com/gtbbztxzal.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtangkazxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cqqwz.cn/gtzczaymls.html

[R60] 只看 HTTP 状态码
来源：http://hz.haohaochexian.top/gtfdxyefxz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtyxbeeaky.html

[R61] 磁盘占用
来源：http://hz.meibo888.top/gtoiapijli.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtnmfromhg.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtlnmbjwvb.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gttimkrjyz.html

[R63] 内存与进程
来源：http://hz.fzhhl.top/gtihlqqtjk.html

free -h;  ps aux | grep nginx
来源：http://hz.havefunace.top/gtmjtmvcbx.html

[R64] 结束进程
来源：http://hz.nanxinkj.top/gtgbsjttgo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtmuqmatjh.html

[R65] 查看端口占用
来源：http://hz.hywenlv.cn/gtrygfafjs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtkshbocyf.html

[R66] 定时任务
来源：http://hz.9152youxi.cn/gtmcgjeajo.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtpzrsgvcs.html

[R67] 生成随机十六进制串
来源：http://hz.yongpay.top/gtvuzrygji.html

openssl rand -hex 16
来源：http://hz.daxiang520.top/gtcunrigeb.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtebfjqknt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtsvqmtqxg.html

[R69] 生成随机密码
来源：http://hz.pycfn.com/gtsffqoozf.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gtwcnxhkpj.html

[R70] 时间戳与互转
来源：http://hz.hysaishi.cn/gtjhoqjyke.html

date +%s;  date -d @1700000000
来源：http://hz.cqqwz.cn/gthkwwvpkw.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtyunfxxcg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.snrcjt.cn/gtaluemdzb.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gthogkhrta.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtcwsqknsc.html

[R73] 分割大日志
来源：http://hz.jinyuanbaomall.cn/gtibfkyvpz.html

split -l 1000 big.log part_
来源：http://hz.haohaochexian.top/gtvfljnhqu.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtodpqzjfc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydjk.org.cn/gtrvbxznbd.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtokumllcr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gtfekymevo.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtwkcesetm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtzfwkfrqg.html

[R77] 读取用户输入
来源：http://hz.hywenlv.cn/gtmamuaogo.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtcivnmnep.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gthwdmcudz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gtbexwondk.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtliijljka.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhaomingkeji.xyz/gtwabjsxgh.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtsdeuekpk.html

time ./run.sh
来源：http://hz.yvedp.cn/gtzjxozegl.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyvvkkyqq.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtxfffurhc.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtyyomjtww.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtintxskkd.html

#include <stdio.h>
来源：http://hz.yj202588.top/gtgsypdgcz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.andypj.xyz/gtitmpjscs.html

[S02] C：变量与格式化输出
来源：http://hz.52xcode.cn/gtabjasuet.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtwsabdkht.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtjmvvvrxm.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtzbsymynw.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gtfejnqbsk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtyfdcpjzc.html

[S05] C：字符串长度
来源：http://hz.jinghuilouyu.cn/gtbugvcvma.html

strlen(s)
来源：http://hz.52xcode.cn/gtymzbxpmu.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtlphckgcy.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtvzebprdj.html

[S07] C：数组遍历求和
来源：http://hz.ivvv.top/gtpfxpwrof.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhengqikj.top/gtserhocmv.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gtwsiuoyzp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtbanfbktf.html

[S09] C：结构体定义与初始化
来源：http://hz.zdqjudy.top/gtjmbrrtfl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gtuvrrrqsn.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtuprpehlx.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtstbatywr.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gttczxdagf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yangfankeji.com/gtbtsszcuq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtkijqggpm.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtdmuxjxnt.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtvfyrmckr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shzxlz.cn/gtpcymdgkx.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtkzxwyevo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.quarkkingdee.top/gtoqnxtqlw.html

[S14] C：枚举
来源：http://hz.andypj.xyz/gtuxijgwvf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtlenuopvb.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtlugkzfrz.html

(double) a / b
来源：http://hz.yj20258888.top/gtktpqlsnu.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtabdmuldb.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtzxvqmsgr.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtfcmytriz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhixingplan.top/gtjtxeuyfv.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gtsqtomkcm.html

int main(int argc, char **argv)
来源：http://hz.birdmap.top/gtjnmxgxak.html

[S19] C：快速排序
来源：http://hz.yangfankeji.com/gtkuotvogy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtduypnpju.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtkgislnhd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtzmcdcssv.html

[S21] C：字符类别判断
来源：http://hz.zhijiandao.cn/gtncpnaaid.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtmmdcjmnc.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtzvvnmglj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gtodrabsgu.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtkwmeslpq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtmbfqbmif.html

[S24] C：获取本地时间
来源：http://hz.cdnleiting.top/gtzwhhwqoq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtptkqgens.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtrptjpmjc.html

memcpy(dst, src, n);
来源：http://hz.jyoumei.cn/gtgdpdavgp.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtmamugede.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangtech.top/gtniwtfggu.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtnaslpdvl.html

const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtcrwuyjcb.html

[S28] C：静态变量
来源：http://hz.xylfe.cn/gtixhhquof.html

static int counter = 0;
来源：http://hz.hnxiangtu.top/gtxwmgeomo.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtsbhbzeau.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jianghu66.top/gthzcpabpx.html

[S30] C：头文件保护
来源：http://hz.zhongyouzk.top/gtvhedscov.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtzfdgmisy.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtydwwweat.html

#endif
来源：http://hz.hammf.cn/gtoiaufaqb.html

[S31] C++：Hello World
来源：http://hz.sysykeji.top/gtkxasqzho.html

#include <iostream>
来源：http://hz.jlsjyb.cn/gtifbhksxi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shuidangran.top/gtmsvlzfow.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtlqbiuswb.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gtkvzktsvp.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtlazooxeh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtvqggaowk.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtxuomsihs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtnmrvyjgv.html

[S35] C++：map
来源：http://hz.gzhubu.top/gtbkihtqzn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gthghlzpyr.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtnjlsxwgh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtxttrpqlb.html

[S37] C++：set
来源：http://hz.yueranfly.top/gtpngwzpkh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtrlofozfm.html

[S38] C++：排序
来源：http://hz.zhoulong.xyz/gtzzosqjes.html

std::sort(v.begin(), v.end());
来源：http://hz.zdqjudy.top/gtzghqxwjd.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtpwvllyui.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtozrfvlbj.html

[S40] C++：查找元素
来源：http://hz.vqdsnc.cn/gtpglzikup.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nwbrower.top/gtpzqpksxt.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtyktcxavk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.0kj1m.cn/gthxonxyww.html

[S42] C++：继承与虚函数
来源：http://hz.aibaodan.cn/gtfwzcnznj.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtklajqoqd.html

[S43] C++：智能指针
来源：http://hz.kuanghao11.cn/gtagfwvvuj.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtibdpxbdt.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtwqxsdryt.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gtcawxexgh.html

[S45] C++：lambda
来源：http://hz.shangyingyoupin.top/gtywjondsj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yvedp.cn/gtkatgedeq.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gteprtyumr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.smart0.xyz/gttkzsnzcx.html

[S47] C++：结构化绑定遍历
来源：http://hz.sysykeji.top/gtgxhymeqc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cqqwz.cn/gtwulkwlmw.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gteffjjzdc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258.top/gtwcidjbvw.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtmupwmucj.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtbbbijkqr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtptaagvhi.html

[S50] C++：格式化数字
来源：http://hz.sweek.top/gtfbjgfuqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtdghcktmu.html

[S51] C++：显式类型转换
来源：http://hz.shuidangran.top/gtewdrbrcn.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtddchxfqc.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258888.top/gtoxmlwyyd.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtjvwyfftg.html

[S53] C++：移动语义
来源：http://hz.316326.xyz/gtixlsesxa.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtxpxtihlr.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtwmiiuzye.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gthwvtdkqh.html

[S55] C++：结构化绑定
来源：http://hz.zdqjudy.top/gtzhmvfgon.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jlsjyb.cn/gtwtzuwhhl.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gtiqfaqqny.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sufxvd.cn/gtsmftysly.html

[S57] C++：编译期常量
来源：http://hz.yuxming.cn/gtohqisqxc.html

constexpr int N = 10;
来源：http://hz.xinyue.icu/gtecnnjklz.html

[S58] C++：命名空间
来源：http://hz.zhengqikj.top/gtrxshrtdk.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtfegdagia.html

[S59] C++：静态断言
来源：http://hz.jqgufenzy.top/gtmtbmojsk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtqtrkpsrs.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtwmtfvcdl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinghuilouyu.cn/gtlnbrpbov.html

================================================================================
来源：http://hz.xuanzx.com/gtbageftna.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtckwibzdz.html

================================================================================
来源：http://hz.wangdashe.top/gtupmbeiew.html

[T01] Kotlin：Hello World
来源：http://hz.tian-w.cn/gttxqubpvp.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtnwjwktac.html

[T02] Kotlin：变量
来源：http://hz.yonumen.top/gtpnlrybry.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gtlxbckkal.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtryevibhj.html

"值: $b"
来源：http://hz.zhengqikj.top/gtbtvdvear.html

[T04] Kotlin：空安全
来源：http://hz.0kj1m.cn/gtpkvingka.html

val n: String? = null;  n?.length
来源：http://hz.iojbl.cn/gtvjkaszvd.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtukuqivhz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtdkixqntx.html

[T06] Kotlin：集合映射
来源：http://hz.sxryk.cn/gtknbmetzd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuanzx.com/gtvqjpyxon.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtpgxktygm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtqoxlwgqg.html

[T08] Kotlin：数据类
来源：http://hz.smart0.xyz/gtptguvkkq.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtymwukxjh.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxinkj.top/gtrbhojwwp.html

fun String.exclaim() = this + "!"
来源：http://hz.shangyingyoupin.top/gttrrtdfhe.html

[T10] Kotlin：默认参数
来源：http://hz.sysykeji.top/gtqorswipx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dianchejie.cn/gtvmcoicdl.html

[T11] Kotlin：协程
来源：http://hz.guowangkeji.top/gtcqfjdotr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtgqinlrqn.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtenacdmqb.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangdashe.top/gtlnudslvh.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtnxhrxvrv.html

val m = mapOf("a" to 1)
来源：http://hz.ehwqpu.com/gtbndgdyrf.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtahujehlc.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtvdkwihdi.html

[T15] Kotlin：接口
来源：http://hz.yuxming.cn/gtrcdhnegz.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtgcjptzgo.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtvmivdtve.html

print("Hello")
来源：http://hz.xuanzx.com/gtalqzqdbw.html

[T17] Swift：变量与常量
来源：http://hz.fengsongda.top/gtsyhlukiv.html

var a = 1;  let b = 2
来源：http://hz.gogol.net.cn/gtwoptcbrm.html

[T18] Swift：字符串插值
来源：http://hz.redwolf501.top/gtnidzufky.html

"值: \(b)"
来源：http://hz.cashguo.top/gtvtrwkyoj.html

[T19] Swift：可选绑定
来源：http://hz.yvedp.cn/gtgtwbxmeg.html

if let n = opt { print(n) }
来源：http://hz.sysykeji.top/gtveybmwrp.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtcdxionbj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtluofigzi.html


<!-- 参考信息 -->