代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.cqqwz.cn/gtfslmwdcz.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtfymhghzg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.andypj.xyz/gtxyoscakv.html

[R33] 捕获错误并提示行号
来源：http://hz.iojbl.cn/gtffoponai.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gtrsmifhyl.html

[R34] 退出时清理
来源：http://hz.sweek.top/gtdjgtyvvx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtxhiqrzok.html

[R35] 后台执行并等待
来源：http://hz.jinqigfzy.top/gttfjilmfp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gtfheeeoug.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtolhgucxf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtgeutnszj.html

[R37] 把输出赋给变量
来源：http://hz.zycfv.cn/gttgrrveyq.html

files=$(ls -1)
来源：http://hz.andypj.xyz/gtrnvcnflc.html

[R38] 管道串联
来源：http://hz.gaohongyu789.top/gtijzjzkeo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gtveapcgvu.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtinxcewhh.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gthbjusqwu.html

[R40] 追加写日志
来源：http://hz.hongshengwenyu.top/gtjxxtgklm.html

echo "log" >> out.log
来源：http://hz.yangfankeji.com/gtlcgvisda.html

[R41] 丢弃输出
来源：http://hz.ydzc1.top/gtgelpdmur.html

cmd >/dev/null 2>&1
来源：http://hz.jqgufenzy.top/gtadvqxtop.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtpvuijflt.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtzoznityg.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtzsdcikns.html

find . -name "*.log" -type f
来源：http://hz.dianchejie.cn/gtmzjtgdof.html

[R44] 按修改时间查找
来源：http://hz.yongpay.top/gtfrnjkqpq.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtoxcxdfzq.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtbuwhlvbe.html

find . -name "*.tmp" -delete
来源：http://hz.hammf.cn/gtbxtkvxzk.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtgxjpvfdp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtiykrgtju.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtrrriegmx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtboizcphj.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtctkxuznw.html

awk '{print $1, $3}' a.txt
来源：http://hz.shzxlz.cn/gtavpdkyfg.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtdogpowqo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xinyue.icu/gtzhkxsgtg.html

[R50] awk 求和
来源：http://hz.cheryme.top/gthhkgaage.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtucpenynj.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtomfhimeu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtemsjdgrh.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gtsvagzgfs.html

wc -l a.txt
来源：http://hz.shzxlz.cn/gtqxyrfhrh.html

[R53] 查看文件头与实时尾
来源：http://hz.sufxvd.cn/gtetnznorq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtjeyyqkrg.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtvxhbponu.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtogjghces.html

[R55] 压缩与解压
来源：http://hz.zhengqikj.top/gtaeklurtq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtkxkxjcky.html

[R56] 远程拷贝
来源：http://hz.daria6918.cn/gtcxdcyowj.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtbtfaynmp.html

[R57] 远程执行命令
来源：http://hz.jianghu66.top/gtnhsdfvmr.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtfmcikwfg.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtlgjnodvu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtchbdgqxr.html

[R59] 发 POST JSON
来源：http://hz.ppjwa.cn/gtayfqlhtr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gthgsgmcjl.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydzc1.top/gtytdetfcd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sufxvd.cn/gtnfolvlwi.html

[R61] 磁盘占用
来源：http://hz.xinyue.icu/gtihgllwkd.html

df -h;  du -sh *
来源：http://hz.kuanghao11.cn/gtordxzlbj.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gtanytauer.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtcoqmfxmb.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtfeenhose.html

free -h;  ps aux | grep nginx
来源：http://hz.xziqi.cn/gtffortjxd.html

[R64] 结束进程
来源：http://hz.shzxlz.cn/gtsibukitv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gtlrqcbgbl.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtrkdsxarz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtezlsihqq.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtpxqyuwff.html

crontab -e;  crontab -l
来源：http://hz.cdnleiting.top/gtfnaduzsf.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtlcrzfzhl.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gtgelikjdo.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtprkcvpuj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtrntiagvu.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtvxqtvvkd.html

head -c 16 /dev/urandom | base64
来源：http://hz.52xcode.cn/gtujqicutk.html

[R70] 时间戳与互转
来源：http://hz.0kj1m.cn/gtuckgqaec.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtukyjogna.html

[R71] 日期格式化
来源：http://hz.yangfankeji.com/gtxtwqnvyi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtecqmubhr.html

[R72] 等待端口就绪
来源：http://hz.svipenyu.cn/gtifzpdtka.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtomizuvvv.html

[R73] 分割大日志
来源：http://hz.andypj.xyz/gtcnwilwqb.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtcvrytjrl.html

[R74] 批量重命名
来源：http://hz.aibaodan.cn/gtloozmxdb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.snrcjt.cn/gtiylaivxn.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtluypbxgc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtipozlcoy.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtixnppytv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtammaisqr.html

[R77] 读取用户输入
来源：http://hz.daria6918.cn/gtrvurmnuz.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtmzqiodtu.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtifjhlejf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.52xcode.cn/gtrxdbjtvc.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gtefoarrwi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtswvxqred.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtulmidkth.html

time ./run.sh
来源：http://hz.ydjk.org.cn/gtszqyfldr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjcjjcxal.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtwlwdwhcw.html

================================================================================
来源：http://hz.cashguo.top/gtrkvacflc.html

[S01] C：Hello World
来源：http://hz.hnxiangtu.top/gtiecyvcgk.html

#include <stdio.h>
来源：http://hz.nanxinkj.top/gtyhfjgxvh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangshuangyany.cn/gtyezdwwoo.html

[S02] C：变量与格式化输出
来源：http://hz.52xcode.cn/gtqtctxdit.html

int a = 10; printf("%d\n", a);
来源：http://hz.xziqi.cn/gtsiyrczfy.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtqimnwqmd.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtztqupcdz.html

[S04] C：字符串复制
来源：http://hz.ehwqpu.com/gtbyzrnjtf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.andypj.xyz/gtuuujgayg.html

[S05] C：字符串长度
来源：http://hz.zhixingplan.top/gtcmbgyqxv.html

strlen(s)
来源：http://hz.zdqjudy.top/gtdrzmchzr.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtqdbtkorb.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtiwrxsdfb.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtrctpprqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtsmsspazh.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtalljlqlo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtnweqfbvz.html

[S09] C：结构体定义与初始化
来源：http://hz.ivvv.top/gtriwmajkv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.smart0.xyz/gtfwaqyesw.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtqljbqmzc.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtwyhsvgdv.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtxbacjrdb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtrxeeatap.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtnzgxeheq.html

fclose(f);
来源：http://hz.quarkkingdee.top/gtwhulbnkd.html

[S12] C：写文件
来源：http://hz.zycfv.cn/gtaeskckwb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhengqikj.top/gtoutssdcb.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtwnfulokx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gttcxqfyxu.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gtpiobbuta.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gtqswnzcdl.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtosnirebq.html

(double) a / b
来源：http://hz.316326.xyz/gtfjegmfpo.html

[S16] C：位操作置位
来源：http://hz.hongshengwenyu.top/gtktwnibpo.html

x |= (1 << 3);
来源：http://hz.zycfv.cn/gtvcaznsya.html

[S17] C：安全拼接字符串
来源：http://hz.ydjk.org.cn/gtetdvrcau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gtnrghozvx.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gtlpwzfkdc.html

int main(int argc, char **argv)
来源：http://hz.chenjidiqi.icu/gtlzjuudwh.html

[S19] C：快速排序
来源：http://hz.sufxvd.cn/gtdowrvsbc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtunkbkhku.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtwwkaqjgc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtprryyyxk.html

[S21] C：字符类别判断
来源：http://hz.redwolf501.top/gtxechnhyh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtoshljmaa.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtksifesvx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xylfe.cn/gtnxzaaamk.html

[S23] C：随机数
来源：http://hz.gotoacloud.top/gtgsffwjrs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtoazdqswl.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtglultkna.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtscedpouw.html

[S25] C：内存拷贝
来源：http://hz.feifeiyinyue.top/gtzqsiqett.html

memcpy(dst, src, n);
来源：http://hz.aibaodan.cn/gtsxtccwfb.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtydobnxzg.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gthqoxnmuo.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtfknzrddm.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtgtpddbrs.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtumraulnu.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtorznqaee.html

[S29] C：变参函数
来源：http://hz.sufxvd.cn/gtqhkgjldc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtsjlwwajz.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtkphwzpsu.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtdbtdagsm.html

#define X_H
来源：http://hz.316326.xyz/gtymqgewea.html

#endif
来源：http://hz.wangdashe.top/gtfkpwnhvg.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtntuodpwm.html

#include <iostream>
来源：http://hz.hywenlv.cn/gtmhcjpcgh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtrkerrtoc.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtikjumcpo.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtjkolngnt.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtprpebfcp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtwfwwbvqy.html

[S34] C++：遍历 vector
来源：http://hz.tian-w.cn/gtaazpmmnp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtmcbfgebg.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtryoowpyz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtmlkokxwt.html

[S36] C++：unordered_map
来源：http://hz.dianchejie.cn/gttzeuhesq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtfbcegfid.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtgfnbicky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtyadtqzdd.html

[S38] C++：排序
来源：http://hz.cashguo.top/gtmnhthlab.html

std::sort(v.begin(), v.end());
来源：http://hz.hongshengwenyu.top/gtfcgilfjv.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gtbolvovwj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jiagoushi.top/gtmbbxhwli.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtpjzcqvha.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtwgvjkzte.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtjnyvulzk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aibaodan.cn/gtzkmormph.html

[S42] C++：继承与虚函数
来源：http://hz.yj202588.top/gtfdnzhhqo.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtyqqutues.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gthdaiztfj.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtsmmgwege.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtrzfywmtk.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtjbmcepae.html

[S45] C++：lambda
来源：http://hz.zhoulong.xyz/gtsvehlens.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangkeji.top/gtdqgagicn.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtwnjrafnc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gttpiibqfa.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gtlqdoejvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtyfnlldaj.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtvolegcnh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtftwcghuj.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gtkfrgcfbm.html

[S49] C++：写文件
来源：http://hz.hywenlv.cn/gtmjcnngel.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gtzdgshabk.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtsnlgknyp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtmkavtcne.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtpwhybtct.html

static_cast<double>(a) / b
来源：http://hz.52xcode.cn/gtskiecjwg.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gttojkvsal.html

int size() const noexcept { return n_; }
来源：http://hz.9152youxi.cn/gtzsiahwjl.html

[S53] C++：移动语义
来源：http://hz.yuanzhike.top/gtlvznejaz.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtyiffgowx.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gtromputsj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtalqvsuma.html

[S55] C++：结构化绑定
来源：http://hz.cucudq.cn/gtgguwkleq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtruvefjah.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtcntfcvsg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.haohaochexian.top/gtslwfztjq.html

[S57] C++：编译期常量
来源：http://hz.cheryme.top/gtdehcslkg.html

constexpr int N = 10;
来源：http://hz.zhoulong.xyz/gtyryqocmw.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gthlkaaflh.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigufen.top/gtjgoujfpg.html

[S59] C++：静态断言
来源：http://hz.jiagoushi.top/gtnzlyvqao.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtcbmxuzep.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtssrencsg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuanzx.com/gthnsprfyd.html

================================================================================
来源：http://hz.pycfn.com/gtpxigpymm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtgcxvsnth.html

================================================================================
来源：http://hz.daria6918.cn/gtjzbtazbq.html

[T01] Kotlin：Hello World
来源：http://hz.zhijiandao.cn/gtcdpnqucb.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtrnsorsup.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtozjhqifz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.mhx1999.top/gtgihvikrd.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gtkzidxbxl.html

"值: $b"
来源：http://hz.c1oappe.top/gtdwsdqksh.html

[T04] Kotlin：空安全
来源：http://hz.gogol.net.cn/gttxagmaar.html

val n: String? = null;  n?.length
来源：http://hz.chenzaomai.com/gtktsnsnun.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtxpplgenr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhiwuduotai.top/gtlmvccird.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gtokwcugqt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.0kj1m.cn/gtlomkycse.html

[T07] Kotlin：集合过滤
来源：http://hz.hysaishi.cn/gtmpgevzsd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jianghu66.top/gtlvtlgphv.html

[T08] Kotlin：数据类
来源：http://hz.jinghuilouyu.cn/gtfnrpdmgo.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtkyiqmzwu.html

[T09] Kotlin：扩展函数
来源：http://hz.sysykeji.top/gttuocybzf.html

fun String.exclaim() = this + "!"
来源：http://hz.sysykeji.top/gtundbpuxp.html

[T10] Kotlin：默认参数
来源：http://hz.chenlongwang.top/gtfaqxkwfw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtfwvvgxyv.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtxffklgts.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gaohongyu789.top/gteqauzkhz.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gtpbqphuic.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhixingplan.top/gtwuodrkpi.html

[T13] Kotlin：只读 Map
来源：http://hz.bjfxy.top/gtnagyybzz.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtjofgblbo.html

[T14] Kotlin：循环
来源：http://hz.zhengqikj.top/gtpayrlviz.html

for (i in 1..10) println(i)
来源：http://hz.hnqzz.top/gtboxvxijx.html

[T15] Kotlin：接口
来源：http://hz.zhiwuduotai.top/gthudhrdow.html

interface Shape { fun area(): Double }
来源：http://hz.feifeiyinyue.top/gttmzawicb.html

[T16] Swift：Hello World
来源：http://hz.zhaomingkeji.xyz/gtvbzjeupj.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtfrszblyi.html

[T17] Swift：变量与常量
来源：http://hz.guowangkeji.top/gttxulwfpm.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtemmhkibv.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtjigkawxy.html

"值: \(b)"
来源：http://hz.zycfv.cn/gtxkizuvjd.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtphcvwscd.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gturvidtct.html

[T20] Swift：数组操作
来源：http://hz.daxiang520.top/gtwmidbqzz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guannengcc.top/gtjhjwfpwd.html

[T21] Swift：遍历
来源：http://hz.xuetiantiany.cn/gtvsaqcynd.html

for x in a { print(x) }
来源：http://hz.daria6918.cn/gtzhbofvfc.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtrdiqtndn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yueranfly.top/gtfcahrdbv.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtrvbftvov.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenlongwang.top/gtpzraknqa.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtmsysrfgy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.birdmap.top/gttqmxqkje.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtcejmmyhd.html

struct P { var x: Int }
来源：http://hz.shzxlz.cn/gtvftwwimd.html

[T26] Swift：类与重写
来源：http://hz.9152youxi.cn/gtbujzwrar.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtxxruzrky.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gtyozpfmmu.html

do { try f() } catch { print(error) }
来源：http://hz.daria6918.cn/gtaaznvryu.html

[T28] Swift：枚举
来源：http://hz.daria6918.cn/gtevngwjdo.html

enum Color { case red, green }
来源：http://hz.0kj1m.cn/gtroyginzi.html

[T29] Swift：guard 提前返回
来源：http://hz.52xcode.cn/gtlnjgjqhz.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtphmmmigh.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtckthquqg.html

protocol Shape { func area() -> Double }
来源：http://hz.yangfankeji.com/gtoqagrlol.html

[T31] Lua：Hello World
来源：http://hz.birdmap.top/gtjqbewnvl.html

print("Hello")
来源：http://hz.andypj.xyz/gtqutgvyio.html

[T32] Lua：局部变量
来源：http://hz.ivvv.top/gtrzzckuid.html

local a = 1
来源：http://hz.zhongyouzk.top/gtzoiekxqu.html

[T33] Lua：表（数组）
来源：http://hz.hfpthk.cn/gteflnnezk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.c1oappe.top/gtratxhhdm.html

[T34] Lua：遍历表
来源：http://hz.chenzaomai.com/gtojsxonlj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtjddpfrdf.html


<!-- 参考信息 -->