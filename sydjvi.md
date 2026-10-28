代发 wailian999

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtnrviubjn.html

[R20] 关联数组（字典）
来源：http://hz.jianghu66.top/gtnzeopyzq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinghuilouyu.cn/gtskdbnkjd.html

[R21] 字符串长度
来源：http://hz.shuidangran.top/gtytznbwfk.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gttzkmmfyo.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtnromviav.html

echo "${s:0:5}"
来源：http://hz.yangfankeji.com/gtizvpfgzc.html

[R23] 字符串替换
来源：http://hz.zhoulong.xyz/gthhkqayew.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtkwzgjixo.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtqfkitucq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtxpcbuwqr.html

[R25] 去后缀 / 去前缀
来源：http://hz.haohaochexian.top/gtqhdxjcdl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigfzy.top/gtacswscis.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtprjrvjdy.html

now=$(date +%F); echo "$now"
来源：http://hz.yj202588.top/gtqwumbxow.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtjrcifekm.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtitbinqlj.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtogeviple.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhaomingkeji.xyz/gtqauhgyqi.html

[R29] 定义函数
来源：http://hz.jianghu66.top/gtnzrvcvag.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zdqjudy.top/gtjmqgqasz.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtrelpjtnw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj202588.top/gtrwtuxrpq.html

[R31] 局部变量
来源：http://hz.ybcxt.top/gtpjxdzfhq.html

f() { local x=1; echo "$x"; }
来源：http://hz.pengpengdd.cyou/gtsfsnugtl.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtmncqkbez.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtaqxwtfat.html

[R33] 捕获错误并提示行号
来源：http://hz.tian-w.cn/gtmhihurxw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yvedp.cn/gtjblhggdj.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtjnbvfybd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtotinoren.html

[R35] 后台执行并等待
来源：http://hz.xuanzx.com/gtplvhspcd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtjvirsuaz.html

[R36] 并发执行多个任务
来源：http://hz.haohaochexian.top/gtpadkwjfw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtwgbwolbx.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtajziwnjx.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtutkuafkm.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtodbfmdhb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yonumen.top/gtxppzigfx.html

[R39] 重定向标准输出与错误
来源：http://hz.chenjidiqi.icu/gtyaymoatk.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtjjljchts.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtbwfzjbar.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtbrokzxnf.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtyrfivbyk.html

cmd >/dev/null 2>&1
来源：http://hz.yj202588.top/gtuecvwria.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtcunleenr.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtdvrhaqgv.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtliowldjf.html

find . -name "*.log" -type f
来源：http://hz.chenlongwang.top/gtdjuvaskm.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtwmfbdaku.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gthlsibvir.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtdpetokch.html

find . -name "*.tmp" -delete
来源：http://hz.zhoulong.xyz/gtcvdthlni.html

[R46] 递归替换文件内容
来源：http://hz.yanxiufei.cn/gtssxmuagj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tianlin.xyz/gtodjcpvit.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtcwaicdzd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yongpay.top/gtgtgyxhqe.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtziqtqiih.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtzlhiocwd.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtolbllafh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gtpieikuqw.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtfghvddtw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtojlpcjro.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtrpzfhoys.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gtmtupdjxz.html

[R52] 统计行数
来源：http://hz.meibo888.top/gtmdbyasuq.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtvetwcvnq.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtqntrazdn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangdashe.top/gtlnahdajf.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtvtervheo.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtlfzryali.html

[R55] 压缩与解压
来源：http://hz.feifeiyinyue.top/gtzydxrumt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtbcrystbp.html

[R56] 远程拷贝
来源：http://hz.pengpengdd.cyou/gtnhngkogs.html

scp file user@host:/path/
来源：http://hz.aizwys.cn/gtsxyqwguy.html

[R57] 远程执行命令
来源：http://hz.sxryk.cn/gtnakijhso.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gtfrjwyrpl.html

[R58] 下载文件
来源：http://hz.daria6918.cn/gtiydoikac.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtkozkjeuv.html

[R59] 发 POST JSON
来源：http://hz.xylfe.cn/gtbujcbuip.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.0kj1m.cn/gtqbywwyya.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtrylrsort.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtflaspusk.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtatlybzaq.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtelxoawgi.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtazhdwxvc.html

du -ah . | sort -rh | head -10
来源：http://hz.ybcxt.top/gtoqbmsxah.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtypspnnwo.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtddpisrtu.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtsvlqfstk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gogol.net.cn/gtsxcgvgvw.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtdakgcuvg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shangyingyoupin.top/gtdwyxfjnc.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtesphxrln.html

crontab -e;  crontab -l
来源：http://hz.hongshengwenyu.top/gtzegrjbhs.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtzwiporzk.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gtlpisakvb.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtuwozkwrj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtwhikmqha.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtnebkxkrg.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gtorhktenx.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gtofrqnmgv.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gttrmebjuh.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtyvpdjsml.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zdqjudy.top/gtofnntatn.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtytlxffre.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tianlin.xyz/gtvajnpxwi.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtwyddmpoi.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtpmofonjf.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtfatmzztb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gtfgyplemp.html

[R75] 导出环境变量
来源：http://hz.jinqigufen.top/gtgffklwfe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dashuyun.cn/gtqajjmtrq.html

[R76] 使用临时文件
来源：http://hz.ydjk.org.cn/gtfwikwzdg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtjxdqaxtu.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtylfvhrkx.html

read -rp "请输入: " ans
来源：http://hz.jqgufenzy.top/gtzzzywaul.html

[R78] 交互式菜单
来源：http://hz.guannengcc.top/gtkihjpnga.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtkwneogfd.html

[R79] 解析命令行选项
来源：http://hz.hammf.cn/gtrhxowrmd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxuanxn.top/gtczcovcgf.html

[R80] 查看脚本执行耗时
来源：http://hz.aibaodan.cn/gtivgahvfq.html

time ./run.sh
来源：http://hz.zhongyouzk.top/gtdfxrjqxp.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthizcumgc.html

S. C / C++ 专题
来源：http://hz.52xcode.cn/gtrnjgfblw.html

================================================================================
来源：http://hz.vqdsnc.cn/gtyueygbrl.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtqumoxpbf.html

#include <stdio.h>
来源：http://hz.zycfv.cn/gtszgpsxdi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtljhchxua.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gtszrcwgiq.html

int a = 10; printf("%d\n", a);
来源：http://hz.sufxvd.cn/gtnrycujst.html

[S03] C：读入整数
来源：http://hz.jinghuilouyu.cn/gtiijomblp.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtgzfkejlz.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtobxchvtx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtqhunbalm.html

[S05] C：字符串长度
来源：http://hz.sufxvd.cn/gtrlufsyfe.html

strlen(s)
来源：http://hz.quarkkingdee.top/gtldywswrl.html

[S06] C：字符串比较
来源：http://hz.cucudq.cn/gtxopyfumi.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gtqhryhhkw.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtufxugvfo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtsegpqmsd.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtnnmwalwg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gtelkddfyc.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gthbqmqrjf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hfpthk.cn/gtryhwnvnc.html

[S10] C：指针与解引用
来源：http://hz.cdnleiting.top/gtjwioehfh.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258.top/gtcpuichec.html

[S11] C：逐行读文件
来源：http://hz.hongshengwenyu.top/gtglcnauff.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aibaodan.cn/gtcagochyo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cqqwz.cn/gtvmzeuhju.html

fclose(f);
来源：http://hz.sxryk.cn/gtjndeshat.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtomngxnqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtrxrdzayh.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtnffxwcrd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtmjxyylgi.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtqpjastsr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.c1oappe.top/gtnbwzbxdz.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtcgquwivy.html

(double) a / b
来源：http://hz.shanyushiyangkeji.top/gtvyjnvlux.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtotcuuvke.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtieikferf.html

[S17] C：安全拼接字符串
来源：http://hz.yanxiufei.cn/gtqosurrns.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtwhyxqpyp.html

[S18] C：命令行参数
来源：http://hz.guowangkeji.top/gthbibexwg.html

int main(int argc, char **argv)
来源：http://hz.haohaochexian.top/gtfkkryxwq.html

[S19] C：快速排序
来源：http://hz.ybcxt.top/gtxbvdznzp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtvdgmdrkh.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtovrwhdjj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtppjrlron.html

[S21] C：字符类别判断
来源：http://hz.ppjwa.cn/gtckblamtt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtsnfiaaez.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtoelwygqv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gthbvqrmwr.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtnyywtuir.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtjlmvdgpk.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtjkbuaill.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cheryme.top/gtlpphkrvk.html

[S25] C：内存拷贝
来源：http://hz.ehwqpu.com/gtfqfldvff.html

memcpy(dst, src, n);
来源：http://hz.haohaochexian.top/gtkxwqvhoe.html

[S26] C：内存清零
来源：http://hz.gotoacloud.top/gtayuptune.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtspiworcw.html

[S27] C：定义常量
来源：http://hz.hfpthk.cn/gtbnhzaomw.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtntsdgoif.html

[S28] C：静态变量
来源：http://hz.yj20258888.top/gtdesxhmsi.html

static int counter = 0;
来源：http://hz.birdmap.top/gtmdhisosm.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gtqydhdvtn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.redwolf501.top/gtgghzncjz.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtxkteeneo.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtptnmouua.html

#define X_H
来源：http://hz.yueranfly.top/gtzalejlxi.html

#endif
来源：http://hz.jinqigufen.top/gtobxplboi.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtkpqhoisu.html

#include <iostream>
来源：http://hz.zhaomingkeji.xyz/gttpnrjljv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtehnhqbha.html

[S32] C++：字符串
来源：http://hz.316326.xyz/gtosommqmp.html

std::string s = "hi";  s += "!";
来源：http://hz.hnxiangtu.top/gtuqbejlnv.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtfilvsuvf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.andypj.xyz/gtobrnamyj.html

[S34] C++：遍历 vector
来源：http://hz.yangfankeji.com/gttrykegvv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.9152youxi.cn/gtwliusopf.html

[S35] C++：map
来源：http://hz.316326.xyz/gtrltjkgly.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtnmazqdsi.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gtdjcyusra.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtuohdygof.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtcyzydmvo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fzhhl.top/gtbklxwyzy.html

[S38] C++：排序
来源：http://hz.yj20258.top/gteldehina.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gtibfaejlm.html

[S39] C++：自定义比较器排序
来源：http://hz.cheryme.top/gtaptomemm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtitgkgqvh.html

[S40] C++：查找元素
来源：http://hz.cheryme.top/gtossylbnu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtcfghfuwa.html

[S41] C++：类与构造函数
来源：http://hz.zhoulong.xyz/gtdcuxfqkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gteujeseao.html

[S42] C++：继承与虚函数
来源：http://hz.yonumen.top/gtlwkmlevg.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtkhsjdbfn.html

[S43] C++：智能指针
来源：http://hz.jlsjyb.cn/gtdgsvbkvp.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gttyqjnzrn.html

[S44] C++：引用传参
来源：http://hz.xylfe.cn/gtldltcfat.html

void inc(int &x) { ++x; }
来源：http://hz.yj20258888.top/gtulkuhkup.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gthfgkerji.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtvwnpstmi.html

[S46] C++：函数模板
来源：http://hz.cheryme.top/gtdmfknnbz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtqdmfgjkx.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhijiandao.cn/gthhnrgycy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xylfe.cn/gtrjvozkdd.html

[S48] C++：逐行读文件
来源：http://hz.yvedp.cn/gtqnyxdpnu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtaxatdney.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtqsetqnyj.html

[S49] C++：写文件
来源：http://hz.chenlongwang.top/gtfojrjuah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinyuanbaomall.cn/gtrvhhcaae.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtalfrtifq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.kuanghao11.cn/gtphcvcdpr.html

[S51] C++：显式类型转换
来源：http://hz.dianchejie.cn/gthrffxbpi.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtbjerthrh.html

[S52] C++：const 与 noexcept
来源：http://hz.gaohongyu789.top/gthdpksuxr.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtafyvkoct.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gthfzzcnjn.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtqlozfonj.html

[S54] C++：异常处理
来源：http://hz.hongshengwenyu.top/gtgnmoeers.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gtllrbszkg.html

[S55] C++：结构化绑定
来源：http://hz.shuidangran.top/gtjpaftxzm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnxiangtu.top/gtliwvpmfr.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtxmuacvcn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ivvv.top/gtoqxetcdm.html

[S57] C++：编译期常量
来源：http://hz.hysaishi.cn/gtgcyugedx.html

constexpr int N = 10;
来源：http://hz.hammf.cn/gtnxytuipa.html

[S58] C++：命名空间
来源：http://hz.cheryme.top/gtcnicenxi.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtgyzbrron.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gtlmsqwycf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtpvqtbmfo.html

[S60] C++：遍历并删除元素
来源：http://hz.cucudq.cn/gtvoyeoylz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daria6918.cn/gtgbxqntod.html

================================================================================
来源：http://hz.jiagoushi.top/gtpaouopir.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aibaodan.cn/gtmtycobak.html

================================================================================
来源：http://hz.pycfn.com/gtnfkykiaw.html

[T01] Kotlin：Hello World
来源：http://hz.cdnleiting.top/gtjjqpxypd.html

println("Hello")
来源：http://hz.bjfxy.top/gtztnelgfr.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtnfmuehgj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtpggspkzi.html

[T03] Kotlin：字符串模板
来源：http://hz.zhengqikj.top/gtwigdkmej.html

"值: $b"
来源：http://hz.yuxming.cn/gtnqdtoodc.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtdetfxdor.html

val n: String? = null;  n?.length
来源：http://hz.cheryme.top/gtfgfpmteo.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtlidnlefw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gtitlasvkt.html

[T06] Kotlin：集合映射
来源：http://hz.aibaodan.cn/gtlabphwor.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ppjwa.cn/gtusxbpepw.html

[T07] Kotlin：集合过滤
来源：http://hz.xziqi.cn/gtzxliucxu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.mhx1999.top/gtiaebdnaz.html

[T08] Kotlin：数据类
来源：http://hz.ydjk.org.cn/gtbizlrhwo.html

data class User(val name: String, val age: Int)
来源：http://hz.shuidangran.top/gtidshwqij.html

[T09] Kotlin：扩展函数
来源：http://hz.feifeiyinyue.top/gtnmchgcfi.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gteybsuotw.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gtdoanarco.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.316326.xyz/gtrkqymcwf.html

[T11] Kotlin：协程
来源：http://hz.yuxming.cn/gtrsuyprru.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxinkj.top/gtsmxveqzv.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtvydikbgt.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gttvcvutaf.html

[T13] Kotlin：只读 Map
来源：http://hz.tanke756.top/gtlkaisqge.html

val m = mapOf("a" to 1)
来源：http://hz.0kj1m.cn/gtcgbftgcl.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gtxbqqfanr.html

for (i in 1..10) println(i)
来源：http://hz.snrcjt.cn/gtreywmcns.html

[T15] Kotlin：接口
来源：http://hz.nanxinkj.top/gtjhhfscet.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtovufeqmt.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtkkznpcdx.html

print("Hello")
来源：http://hz.sxryk.cn/gtyjszgruc.html

[T17] Swift：变量与常量
来源：http://hz.jiagoushi.top/gtpxzucmgb.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtkuwozqnf.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtkghcqiml.html

"值: \(b)"
来源：http://hz.daria6918.cn/gthjrqvata.html

[T19] Swift：可选绑定
来源：http://hz.yangfankeji.com/gtfaiguoif.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gteculzibo.html

[T20] Swift：数组操作
来源：http://hz.fzhhl.top/gttxmurizz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinyuanbaomall.cn/gtzckjpowj.html

[T21] Swift：遍历
来源：http://hz.hfpthk.cn/gtcjtwyaxz.html

for x in a { print(x) }
来源：http://hz.jianghu66.top/gtmrbbgird.html

[T22] Swift：字典
来源：http://hz.bjfxy.top/gtutjmhijb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.bjfxy.top/gtzrjqpved.html


<!-- 参考信息 -->