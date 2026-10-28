代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gogol.net.cn/gtmyshvfsn.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtleccmfpf.html

now=$(date +%F); echo "$now"
来源：http://hz.mhx1999.top/gtmvrmuelg.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtgxydxpos.html

echo $((1 + 2 * 3))
来源：http://hz.jinqigufen.top/gtaoeebdgf.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtqjueebvb.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtxbbawddk.html

[R29] 定义函数
来源：http://hz.cdnleiting.top/gtjwihdnfv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtsgkypesq.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtfebnwdsk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gtvoqrllgy.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gtwhowdbca.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhongyouzk.top/gtdermymzv.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtkuaxfkft.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtyzvkecpk.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtsmngmdnd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hammf.cn/gtafjbuolz.html

[R34] 退出时清理
来源：http://hz.shanyushiyangkeji.top/gtaqgjaohq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtohfqyejs.html

[R35] 后台执行并等待
来源：http://hz.feifeiyinyue.top/gtwkqnbqhb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtjuwgnryj.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gtiqrnyqfe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aibaodan.cn/gttqrvptse.html

[R37] 把输出赋给变量
来源：http://hz.mhx1999.top/gtaytnxrny.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtuwtifjmt.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtpnqlgqua.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jyoumei.cn/gtokjcvgtk.html

[R39] 重定向标准输出与错误
来源：http://hz.zdqjudy.top/gtjenfhbej.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtueqctcve.html

[R40] 追加写日志
来源：http://hz.yj20258.top/gtljohlpuu.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtniggfidp.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtrmgewuda.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtqvemzdfy.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtwsynxvqy.html

wc -l < a.txt
来源：http://hz.daria6918.cn/gtfmbnffai.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtqelacjtt.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtjsyshwsd.html

[R44] 按修改时间查找
来源：http://hz.ivvv.top/gtbtexwdjd.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtzwadqwrq.html

[R45] 批量删除
来源：http://hz.gotoacloud.top/gtiajyoyww.html

find . -name "*.tmp" -delete
来源：http://hz.shzxlz.cn/gtejkytkrb.html

[R46] 递归替换文件内容
来源：http://hz.zdqjudy.top/gttycmmoyz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtzwivraqx.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gttsyozvsh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yangfankeji.com/gtyucccoxd.html

[R48] awk 取指定列
来源：http://hz.gaohongyu789.top/gtepoaxzxq.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gtciwmcxcr.html

[R49] awk 带条件
来源：http://hz.tian-w.cn/gtaujcjvsv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuanzhike.top/gtfykydaay.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtamxbvhmz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gthaesaiht.html

[R51] 排序去重取前几
来源：http://hz.jiagoushi.top/gtnyqtvocm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hysaishi.cn/gtrihlaktg.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtkdxserag.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtlgechwhg.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtszctmfgf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gtgmyctdqw.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtwykcpwzw.html

diff a.txt b.txt
来源：http://hz.dashuyun.cn/gtpruaribb.html

[R55] 压缩与解压
来源：http://hz.9152youxi.cn/gtzzjzpvvy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gtzqixwxsr.html

[R56] 远程拷贝
来源：http://hz.meibo888.top/gtbugowfsc.html

scp file user@host:/path/
来源：http://hz.zhiwuduotai.top/gtqkacywuj.html

[R57] 远程执行命令
来源：http://hz.sxryk.cn/gtnvnmrdor.html

ssh user@host 'uptime'
来源：http://hz.zhiwuduotai.top/gtvdxdhrwa.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtzxzpvmaq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtetsmbhjf.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtznwmvkqx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtnawjhvpg.html

[R60] 只看 HTTP 状态码
来源：http://hz.ybcxt.top/gtwpoykacu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtuxxqqred.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtlovezdxs.html

df -h;  du -sh *
来源：http://hz.dianchejie.cn/gtqhluwojv.html

[R62] 找最占空间的文件
来源：http://hz.xuetiantiany.cn/gttfsxkrij.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtlnskxzod.html

[R63] 内存与进程
来源：http://hz.guowangkeji.top/gthbgwibpt.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gtwypszjmd.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtnwadjxii.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtpubxrjdv.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtcudrwxcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtlyrpjcpt.html

[R66] 定时任务
来源：http://hz.daria6918.cn/gtwpwycdwo.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gtaactbqsi.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtyicboovo.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gthbbnonsl.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gtnbazemrt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtpjirfean.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtlnwxoppf.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtmheufego.html

[R70] 时间戳与互转
来源：http://hz.ehwqpu.com/gtjdrjqqeq.html

date +%s;  date -d @1700000000
来源：http://hz.jinghuilouyu.cn/gtvxtphwnf.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtkkugexzp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhongyouzk.top/gtdozbxphw.html

[R72] 等待端口就绪
来源：http://hz.tianlin.xyz/gtxafsvivr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cheryme.top/gtrtwwexhw.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gtyoltnqqp.html

split -l 1000 big.log part_
来源：http://hz.ydzc1.top/gtxgqjbbkx.html

[R74] 批量重命名
来源：http://hz.316326.xyz/gtwxqiiayw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtwbgvpeww.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtlrgvscdz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtnlvhdgkw.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtyuiccmhx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtzidippur.html

[R77] 读取用户输入
来源：http://hz.hnqzz.top/gthkfapana.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gteoihsoiv.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gtakolcrif.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtplqnjtac.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtghqgvrhf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gthtsjhwzm.html

[R80] 查看脚本执行耗时
来源：http://hz.birdmap.top/gtcnqptwrp.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtkgeuladr.html

================================================================================
来源：http://hz.zhixingplan.top/gtglugxxth.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtjxbrgugn.html

================================================================================
来源：http://hz.yueranfly.top/gtiwrdiagt.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gthfogmvec.html

#include <stdio.h>
来源：http://hz.jinyuanbaomall.cn/gtyxodpubo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtnskukqvc.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gtnyutmxja.html

int a = 10; printf("%d\n", a);
来源：http://hz.gotoacloud.top/gtqelcrewj.html

[S03] C：读入整数
来源：http://hz.dashuyun.cn/gtgwmgmvgb.html

int x; scanf("%d", &x);
来源：http://hz.c1oappe.top/gtmarhklpn.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtyciydgfc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtkwqhthfp.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtyvrfixnd.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtpmbwrxtj.html

[S06] C：字符串比较
来源：http://hz.jiagoushi.top/gtigvfcfjc.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtoagvppiz.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtcfwimvbf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtatnhdnne.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtaysgxeeo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yongpay.top/gtpbalbhzi.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtxknsfgnm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtdideigyc.html

[S10] C：指针与解引用
来源：http://hz.316326.xyz/gthcmzdppi.html

int *p = &a;  *p = 5;
来源：http://hz.yanxiufei.cn/gtrnspeqtf.html

[S11] C：逐行读文件
来源：http://hz.cashguo.top/gtptlrlifx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtcmjsrvnk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.kuanghao11.cn/gtotomfsfu.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtjsvttgpp.html

[S12] C：写文件
来源：http://hz.ppjwa.cn/gtrltcqudc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtbvimvufz.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtzgrwvwqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gtqgtaqcqr.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtxcwajybs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenlongwang.top/gtkiticgtp.html

[S15] C：类型转换
来源：http://hz.chenzaomai.com/gtbubylerq.html

(double) a / b
来源：http://hz.nanxinkj.top/gttecxhxrk.html

[S16] C：位操作置位
来源：http://hz.zdqjudy.top/gtolbguzgl.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtavnmcvji.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gtzsvbgwny.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtzqkgnmsy.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtsrcucrnv.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtoijgtltq.html

[S19] C：快速排序
来源：http://hz.sufxvd.cn/gttnntlyng.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtfraerxon.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gtrxmvqwgd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtnezvlpvx.html

[S21] C：字符类别判断
来源：http://hz.hnxiangtu.top/gthijfemxl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangshuangyany.cn/gtjbeszaui.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gteludqffs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtchrzshjj.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtpfabbagr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtljtbfjuh.html

[S24] C：获取本地时间
来源：http://hz.shuidangran.top/gtdyqqpexo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangkeji.top/gtrowxpgyz.html

[S25] C：内存拷贝
来源：http://hz.gaohongyu789.top/gtaqjhfzbc.html

memcpy(dst, src, n);
来源：http://hz.316326.xyz/gtprorbibm.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtewwwtxem.html

memset(a, 0, sizeof a);
来源：http://hz.ydjk.org.cn/gtskyyqxgp.html

[S27] C：定义常量
来源：http://hz.nwbrower.top/gtrrvsozet.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gtwmgdiymh.html

[S28] C：静态变量
来源：http://hz.gotoacloud.top/gteebuzcsl.html

static int counter = 0;
来源：http://hz.jqgfzy.top/gtzovfenpv.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtbneoofuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtdrzlkccz.html

[S30] C：头文件保护
来源：http://hz.xylfe.cn/gtmgcxnfji.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtidlcdytk.html

#define X_H
来源：http://hz.svipenyu.cn/gtjvrwpxop.html

#endif
来源：http://hz.sxryk.cn/gtalptxsze.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtifndmghq.html

#include <iostream>
来源：http://hz.hywenlv.cn/gtjgnutgva.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gttaxfzttn.html

[S32] C++：字符串
来源：http://hz.cdnleiting.top/gtzqjsirxr.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gtrivkpffz.html

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gthtzmtaim.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtxefuclvq.html

[S34] C++：遍历 vector
来源：http://hz.tanke756.top/gtwvozfoar.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xylfe.cn/gtrxggmkut.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gtqkicmpoy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtqizbclzo.html

[S36] C++：unordered_map
来源：http://hz.yuanzhike.top/gtdjdoxjjc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtuzfrkzbt.html

[S37] C++：set
来源：http://hz.andypj.xyz/gtvtczphgq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtslngtxlk.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtsifhnhcg.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtwnzfverx.html

[S39] C++：自定义比较器排序
来源：http://hz.daria6918.cn/gtvqwecuns.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtxurheghj.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtnpemopdp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yongpay.top/gtrseslufl.html

[S41] C++：类与构造函数
来源：http://hz.zhoulong.xyz/gtmbxgvzsw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinghuilouyu.cn/gtutwhstho.html

[S42] C++：继承与虚函数
来源：http://hz.ybcxt.top/gtpmgqtmck.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtqrpfyfel.html

[S43] C++：智能指针
来源：http://hz.hywenlv.cn/gtvvdxpyds.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtyntgqndj.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtxcknchnv.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gtxisjsvwc.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtoskfswli.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gthwlqhwaq.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtsptiqcfu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gtugbvcvcb.html

[S47] C++：结构化绑定遍历
来源：http://hz.haohaochexian.top/gtanejhykx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.bjfxy.top/gtfvbgwgtb.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtuljurhcd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gtmntokatq.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtaqbepntp.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtzbbdfiao.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gtirohoqrt.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gthlcpnvna.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtykbpjaik.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtrpkgktvq.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtdapsrsfo.html

[S52] C++：const 与 noexcept
来源：http://hz.yonumen.top/gtfixaulei.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtsjltuwvg.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gttvscixtd.html

std::vector<int> w = std::move(v);
来源：http://hz.ehwqpu.com/gtsfrtogof.html

[S54] C++：异常处理
来源：http://hz.quarkkingdee.top/gtzxrtwruh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gteqdtshuu.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtqsyaltin.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxuanxn.top/gtxnhghwbn.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtiefsuxtv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.smart0.xyz/gtnsxlvafv.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtpzobrijz.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gtdjjqdtzo.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtuirggwen.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtcdqzbzez.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gtkujbqyto.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xingfuxueyuan.xyz/gtmykwnljm.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gthjgwsqzh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtwsgosnag.html

================================================================================
来源：http://hz.jianghu66.top/gthbumnpnm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtbidczwye.html

================================================================================
来源：http://hz.tanke756.top/gthuqcuuqb.html

[T01] Kotlin：Hello World
来源：http://hz.sweek.top/gtyyblgtim.html

println("Hello")
来源：http://hz.yuanzhike.top/gtzepezlqn.html

[T02] Kotlin：变量
来源：http://hz.havefunace.top/gtfjbxggci.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtndpxrlpe.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtmlirbjsu.html

"值: $b"
来源：http://hz.c1oappe.top/gtgwdpwohk.html

[T04] Kotlin：空安全
来源：http://hz.hongshengwenyu.top/gtkllquhiz.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtrutfgyvi.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtgktlnpqw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gtsjpknqgy.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gttgzstjqw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtujhppqef.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtgluwleai.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtinewmwmm.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtezktomtt.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gthhqdwwnx.html

[T09] Kotlin：扩展函数
来源：http://hz.zhoulong.xyz/gtbtynrwny.html

fun String.exclaim() = this + "!"
来源：http://hz.sysykeji.top/gtbelhxbud.html

[T10] Kotlin：默认参数
来源：http://hz.xylfe.cn/gthegiyhra.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gthkbflkqu.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtywceuprd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shuidangran.top/gtreijgjrb.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtancvjevg.html

val (a, b) = Pair(1, 2)
来源：http://hz.yonumen.top/gtwjukgrvu.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gthjjsfseq.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtftvqzzon.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtnbnuqasf.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtthjmbhtj.html

[T15] Kotlin：接口
来源：http://hz.chenzaomai.com/gtbisrszxh.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtzxoduxlk.html

[T16] Swift：Hello World
来源：http://hz.gogol.net.cn/gtvuabfmik.html

print("Hello")
来源：http://hz.zhengqikj.top/gtvozwhuko.html

[T17] Swift：变量与常量
来源：http://hz.yvedp.cn/gtlsrbtquq.html

var a = 1;  let b = 2
来源：http://hz.shanyushiyangkeji.top/gtxpjqcoyv.html

[T18] Swift：字符串插值
来源：http://hz.wangshuangyany.cn/gtainzujtt.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gtmazpkcjn.html

[T19] Swift：可选绑定
来源：http://hz.yvedp.cn/gtehwslqxw.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtpoaoybuq.html

[T20] Swift：数组操作
来源：http://hz.cucudq.cn/gtnkolgdoh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gttorlafbo.html

[T21] Swift：遍历
来源：http://hz.dianchejie.cn/gtjtjlzxkn.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gthyymewbk.html

[T22] Swift：字典
来源：http://hz.jianghu66.top/gtjveqachk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnxiangtu.top/gtczstqdbj.html

[T23] Swift：函数
来源：http://hz.guowangkeji.top/gtsrwvfsjn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jianghu66.top/gtbufkqnop.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtoupgubsw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtualtcany.html

[T25] Swift：结构体
来源：http://hz.svipenyu.cn/gtuihowvge.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtnkrotnqg.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtwegqqfdx.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtjiokqgrf.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtzspgeosn.html

do { try f() } catch { print(error) }
来源：http://hz.jqgfzy.top/gtwlaodcmk.html

[T28] Swift：枚举
来源：http://hz.chenjidiqi.icu/gtfkjayusf.html

enum Color { case red, green }
来源：http://hz.smart0.xyz/gtjfdfteme.html


<!-- 参考信息 -->