代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtvzrmwefb.html

[R24] 大小写转换
来源：http://hz.quarkkingdee.top/gtmiohydmz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtnnprktpo.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuanzx.com/gtwmglxtyt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtfdqzazcj.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gthurolcyk.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtoxgdfpzt.html

[R27] 算术展开
来源：http://hz.cashguo.top/gtjcqohhkz.html

echo $((1 + 2 * 3))
来源：http://hz.zhengqikj.top/gtspwvojxo.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtydyttres.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtccbzqacz.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtfioihwuw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gttdumgfsl.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gteapgjkfy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangkeji.top/gtercustdo.html

[R31] 局部变量
来源：http://hz.hammf.cn/gthskghrfc.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtbrycepnp.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtjvndsoor.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.andypj.xyz/gtkrabwkls.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtlnpmeazv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtpvhrrhwu.html

[R34] 退出时清理
来源：http://hz.shuidangran.top/gtvddsqxzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gtwzbzqbus.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtypbalbct.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtrlfqxvwn.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtdkcqbmjj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xinyue.icu/gtnhtxlnot.html

[R37] 把输出赋给变量
来源：http://hz.chenlongwang.top/gtyemvxlqc.html

files=$(ls -1)
来源：http://hz.ehwqpu.com/gtlecyhkqp.html

[R38] 管道串联
来源：http://hz.chenlongwang.top/gttighnwxk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtevkltseu.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtjqhsixig.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gtgorvdsjr.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtdmhgwazw.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtdcbajpdz.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtcebqiwdl.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gtjjqhuaom.html

[R42] 输入重定向
来源：http://hz.xuetiantiany.cn/gtqvqmzwbl.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtxjzdnalh.html

[R43] 按名字查找文件
来源：http://hz.tianlin.xyz/gtjclwtpkz.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gtoakzfzul.html

[R44] 按修改时间查找
来源：http://hz.jiagoushi.top/gtozerblaf.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gtqirkznft.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gttzfdihmn.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtwrthtfoh.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gtzntybmkn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtdzcktnjy.html

[R47] sed 单行替换
来源：http://hz.ybcxt.top/gtzomxotyi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtngvjldop.html

[R48] awk 取指定列
来源：http://hz.ehwqpu.com/gtkzirdsds.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtoysjkjpj.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtqoacowax.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtrnvaxnxv.html

[R50] awk 求和
来源：http://hz.hfpthk.cn/gtislvkfzo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtbgpbllmz.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gthhtgzzzi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gtddruvjih.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtbczghles.html

wc -l a.txt
来源：http://hz.ydjk.org.cn/gtcywfakzh.html

[R53] 查看文件头与实时尾
来源：http://hz.52xcode.cn/gtiegnphpg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgufenzy.top/gtswviwnyf.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtqsklcyiy.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gtabjjcrnp.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtiyhvlgbq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gtgqdsbrqv.html

[R56] 远程拷贝
来源：http://hz.cucudq.cn/gtxykyvcnr.html

scp file user@host:/path/
来源：http://hz.xinyue.icu/gtvzlzoeul.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gttzgqmhsx.html

ssh user@host 'uptime'
来源：http://hz.jyoumei.cn/gtikrkyqkq.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtssvaaevj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtgvlwvhii.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtzjmnvlxg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtjyclrada.html

[R60] 只看 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtzxmdwgna.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj20258888.top/gtiicfejym.html

[R61] 磁盘占用
来源：http://hz.yuanzhike.top/gtxzuwuqyg.html

df -h;  du -sh *
来源：http://hz.quarkkingdee.top/gtfezlpsuc.html

[R62] 找最占空间的文件
来源：http://hz.vqdsnc.cn/gttlpdfrqj.html

du -ah . | sort -rh | head -10
来源：http://hz.gzhubu.top/gtmrmgchzx.html

[R63] 内存与进程
来源：http://hz.snrcjt.cn/gtbcjtaxhe.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gtpuwkijww.html

[R64] 结束进程
来源：http://hz.redwolf501.top/gtscwfygpe.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gtsjbheljn.html

[R65] 查看端口占用
来源：http://hz.sweek.top/gttmbqlhap.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhiwuduotai.top/gtekxmjech.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtbufovfco.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtojqredld.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtyczpbpbz.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtmcqqfzyy.html

[R68] 计算文件校验值
来源：http://hz.guowangkeji.top/gtozmgclty.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhongyouzk.top/gtajkcobzr.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtqjpslksr.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtbgnauwby.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtqwvdxctg.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtoccggeqk.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtsovhfhys.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtidbuvvdb.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtspkugplp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtjvopslyz.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtkriqouip.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gttgkxnihb.html

[R74] 批量重命名
来源：http://hz.yuxming.cn/gtlfpvjsqo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtpcwziirj.html

[R75] 导出环境变量
来源：http://hz.fzhhl.top/gthrilebns.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhengqikj.top/gtfnmnzfhu.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gtcfpriszq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtbcrtpdlj.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtiejjcomg.html

read -rp "请输入: " ans
来源：http://hz.gaohongyu789.top/gthrvnkqsg.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtruabnrfo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtqhhxnqaz.html

[R79] 解析命令行选项
来源：http://hz.yj20258.top/gtcavzqxwx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtmrudrock.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtrjcmyykv.html

time ./run.sh
来源：http://hz.yuxming.cn/gtafpiugjo.html

================================================================================
来源：http://hz.yangfankeji.com/gthsrgslgv.html

S. C / C++ 专题
来源：http://hz.iojbl.cn/gtvgabctyh.html

================================================================================
来源：http://hz.jqgfzy.top/gtfwchdtjh.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtryhgttmb.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtyoypctgo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtozmecrqq.html

[S02] C：变量与格式化输出
来源：http://hz.guowangkeji.top/gthknzeilp.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gthwexpaac.html

[S03] C：读入整数
来源：http://hz.nanxinkj.top/gtmhjzskiq.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtrvqqsyam.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtrrbfabmz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.kuanghao11.cn/gtqbicvxze.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtmlzyhhra.html

strlen(s)
来源：http://hz.cashguo.top/gtdvkdmoqy.html

[S06] C：字符串比较
来源：http://hz.nanxinkj.top/gtfhtdbmvz.html

strcmp(a, b) == 0
来源：http://hz.mhx1999.top/gtdnexlawx.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtibonqcte.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj202588.top/gtklfxtlaa.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtugyxfils.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtfxhwdrwh.html

[S09] C：结构体定义与初始化
来源：http://hz.jinyuanbaomall.cn/gtgqnmmdfi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxinkj.top/gtfmbckkov.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtnmbjcawe.html

int *p = &a;  *p = 5;
来源：http://hz.wangdashe.top/gtjetqmqlg.html

[S11] C：逐行读文件
来源：http://hz.jinqigufen.top/gtthlesnxx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gotoacloud.top/gtpqgmadvv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtwbzwwdxq.html

fclose(f);
来源：http://hz.yj20258.top/gtupvwixva.html

[S12] C：写文件
来源：http://hz.hammf.cn/gtujoxgdxg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtfquvxift.html

[S13] C：宏定义
来源：http://hz.zhoulong.xyz/gtqoitncye.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gtskgbfjio.html

[S14] C：枚举
来源：http://hz.cqqwz.cn/gtbszbvrqg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gtgyamkuip.html

[S15] C：类型转换
来源：http://hz.cqqwz.cn/gtvwbcfspl.html

(double) a / b
来源：http://hz.ybcxt.top/gtkiglfupw.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtiouuqjmj.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtnghgsgqa.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gtgukkxneo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtiwlpjjqk.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtarimtoeu.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtjjapgweu.html

[S19] C：快速排序
来源：http://hz.yuxming.cn/gtirconpwy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gthgjlhdfy.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtsvogitcs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtjdxngler.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gtnrncveba.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xinyue.icu/gtbtopuhhr.html

[S22] C：字符串转数字
来源：http://hz.guowangkeji.top/gtcfqxmuwf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtslhvrjeb.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtwduivbhi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shangyingyoupin.top/gtlprvcuti.html

[S24] C：获取本地时间
来源：http://hz.xuanzx.com/gtjfimcnaa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.feifeiyinyue.top/gtwnoicinu.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtbyinbdtu.html

memcpy(dst, src, n);
来源：http://hz.aibaodan.cn/gtzrqacwob.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtilmnxymm.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtkuumwtkf.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtmdxnabdm.html

const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtligrzkza.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtnmywnxau.html

static int counter = 0;
来源：http://hz.guannengcc.top/gtmyhluakm.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtgzkrsrwv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenzaomai.com/gtwtzrdidn.html

[S30] C：头文件保护
来源：http://hz.xylfe.cn/gtikasmbem.html

#ifndef X_H
来源：http://hz.mhx1999.top/gtwmssgrep.html

#define X_H
来源：http://hz.jinqigufen.top/gtbzhripge.html

#endif
来源：http://hz.meibo888.top/gtpjunpvpw.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtjmphpgzw.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gtpkoiiwce.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhoulong.xyz/gtsifagbro.html

[S32] C++：字符串
来源：http://hz.jinghuilouyu.cn/gtxtcjecet.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtincrdhkx.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtlpydwtkb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtvumuocwy.html

[S34] C++：遍历 vector
来源：http://hz.dashuyun.cn/gtvktplaaq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gtcsbvsvzq.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtwjrlzmoq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtvfgwxjyu.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtgwdxitxp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtgvfzdcxd.html

[S37] C++：set
来源：http://hz.gogol.net.cn/gtpadhtwtp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.9152youxi.cn/gtwwgakfue.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtjynxybsp.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gttqugorrd.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtdwgjosez.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhengqikj.top/gtfvydbkqh.html

[S40] C++：查找元素
来源：http://hz.haohaochexian.top/gtimryqdti.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtlztjkcvf.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gthlsphxmq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnqzz.top/gtpwkbflpc.html

[S42] C++：继承与虚函数
来源：http://hz.jinghuilouyu.cn/gtnqplycsi.html

class B : public Base { public: void f() override {} };
来源：http://hz.yonumen.top/gtyfuzynuu.html

[S43] C++：智能指针
来源：http://hz.aibaodan.cn/gtqsyrojpo.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenlongwang.top/gtaqafhjac.html

[S44] C++：引用传参
来源：http://hz.yonumen.top/gtobarhiii.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtpglkchjv.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtakfeumxo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shangyingyoupin.top/gtuawkhygs.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtvotblmed.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhixingplan.top/gtdrcqrgic.html

[S47] C++：结构化绑定遍历
来源：http://hz.tanke756.top/gtufzxkcwt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtgldetytz.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtuwwaltmx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtuwjqegwd.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtzsbtjanm.html

[S49] C++：写文件
来源：http://hz.yanxiufei.cn/gtjtctxiwc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yvedp.cn/gtdihxvabf.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtbdxkcmaj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gthrrgdsms.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtdlnteqll.html

static_cast<double>(a) / b
来源：http://hz.jqgfzy.top/gtmiedlbyc.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtywjdjogj.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gtvnfjenif.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtdfxrodhl.html

std::vector<int> w = std::move(v);
来源：http://hz.yongpay.top/gtsghlcpot.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtqmqigazd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtkiutrmuo.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtmpndcygh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jyoumei.cn/gtvrqtitgs.html

[S56] C++：optional
来源：http://hz.meibo888.top/gtmgpvcwve.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtbbmuzvdp.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gthkdralkt.html

constexpr int N = 10;
来源：http://hz.jqgufenzy.top/gtglewxjgg.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtiwzejeus.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtwkithkww.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtykpiywds.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtgzruapyy.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gtsixxuehl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtntqiiczh.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjstdufbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhaomingkeji.xyz/gthljpsohi.html

================================================================================
来源：http://hz.chenzaomai.com/gtfunjsefo.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtpjtibxnr.html

println("Hello")
来源：http://hz.meibo888.top/gttsuouaqx.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtiliicqtv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtoasmnjag.html

[T03] Kotlin：字符串模板
来源：http://hz.zhengqikj.top/gtuxpernmd.html

"值: $b"
来源：http://hz.yvedp.cn/gtylvhflte.html

[T04] Kotlin：空安全
来源：http://hz.sxryk.cn/gthnipjuep.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtlbyaqlja.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gthknyjuyo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fzhhl.top/gtcxplfqib.html

[T06] Kotlin：集合映射
来源：http://hz.gotoacloud.top/gtrirgdhba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gtksnnsndr.html

[T07] Kotlin：集合过滤
来源：http://hz.aibaodan.cn/gtlqvttekt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gtvtfxrvjm.html

[T08] Kotlin：数据类
来源：http://hz.bjfxy.top/gtqiugzdoy.html

data class User(val name: String, val age: Int)
来源：http://hz.sweek.top/gtsnmdpsrj.html

[T09] Kotlin：扩展函数
来源：http://hz.sufxvd.cn/gteobrlcra.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtgwcctzde.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtyhqjsjbr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtgyubhkns.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtxrjlulid.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtqfxhmmpv.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258888.top/gtlnhyerkx.html

val (a, b) = Pair(1, 2)
来源：http://hz.gaohongyu789.top/gtcjzzmgra.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtjxrxhytz.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtkiuseeto.html

[T14] Kotlin：循环
来源：http://hz.yanxiufei.cn/gtjcbhwztx.html

for (i in 1..10) println(i)
来源：http://hz.cheryme.top/gtztoysgog.html

[T15] Kotlin：接口
来源：http://hz.cucudq.cn/gtgmhlaequ.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtgybusylc.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtghwmenye.html

print("Hello")
来源：http://hz.fengsongda.top/gtizplmrvz.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtdehxutfi.html

var a = 1;  let b = 2
来源：http://hz.yueranfly.top/gtxfcotroj.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gthbueyhhx.html

"值: \(b)"
来源：http://hz.yuxming.cn/gtemrewfya.html

[T19] Swift：可选绑定
来源：http://hz.smart0.xyz/gtymalmtjo.html

if let n = opt { print(n) }
来源：http://hz.jinqigufen.top/gtnoamyutt.html

[T20] Swift：数组操作
来源：http://hz.yj202588.top/gtuspyvnhl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtiglzuarg.html

[T21] Swift：遍历
来源：http://hz.hongshengwenyu.top/gtcrliuxsq.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtbizpejol.html

[T22] Swift：字典
来源：http://hz.0kj1m.cn/gtinfhmvso.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangtech.top/gtqedustqy.html

[T23] Swift：函数
来源：http://hz.yuanzhike.top/gtavhdgajn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhoulong.xyz/gthkckmpex.html

[T24] Swift：闭包
来源：http://hz.hysaishi.cn/gtxtmmmbdg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.quarkkingdee.top/gtvgiaismo.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gtgfceqlli.html

struct P { var x: Int }
来源：http://hz.xuanzx.com/gtzcewkeik.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtmoezqmam.html

class A: Base { override func f() {} }
来源：http://hz.pycfn.com/gtypefthie.html


<!-- 参考信息 -->