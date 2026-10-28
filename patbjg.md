代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cheryme.top/gtlmzwgate.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtdddmunre.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pengpengdd.cyou/gtrmrmyufb.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gtfzbqhldj.html

echo "${#arr[@]}"
来源：http://hz.ehwqpu.com/gtvewwsrnt.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtvpjsjtlb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenlongwang.top/gtezbhszbk.html

[R21] 字符串长度
来源：http://hz.shangyingyoupin.top/gtzkrwifjs.html

echo "${#s}"
来源：http://hz.yj20258.top/gtmrzwesqk.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtuzkazlmf.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtaqfttsjz.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtwbahwqys.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtbusnzesv.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtmtyodmuq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtfhfbzbmo.html

[R25] 去后缀 / 去前缀
来源：http://hz.gaohongyu789.top/gtdnzwkfnj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj202588.top/gtnvbhprlq.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtjjxcojgx.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtocjhozsh.html

[R27] 算术展开
来源：http://hz.fengsongda.top/gtifeptqat.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtmirrecik.html

[R28] 浮点运算
来源：http://hz.ybcxt.top/gtturdnjgw.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gtnmzwpylw.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtkjbzktsy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hywenlv.cn/gtspjlrxav.html

[R30] 函数返回状态码
来源：http://hz.hysaishi.cn/gtaznhxklb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtpquuxouf.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtqctsydnt.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtfkgoldxy.html

[R32] 参数个数校验
来源：http://hz.ydjk.org.cn/gtglbxxlsy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtmwiphnbe.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtcmditnoh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtmdhofsqf.html

[R34] 退出时清理
来源：http://hz.guannengcc.top/gthtgzvqrg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtmehdvmqm.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gtiihuedby.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cqqwz.cn/gtpkspjbyo.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtkkbtoizy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gthufludqg.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtfaecrdlb.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtswklgioi.html

[R38] 管道串联
来源：http://hz.guowangkeji.top/gtccpmwzmk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuanzx.com/gtpfszhcfp.html

[R39] 重定向标准输出与错误
来源：http://hz.guowangkeji.top/gtegniekfe.html

cmd > out.log 2>&1
来源：http://hz.daria6918.cn/gteijzvtgu.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtvblibvlf.html

echo "log" >> out.log
来源：http://hz.tianlin.xyz/gtbbuzawsg.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtonrpoqck.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gthswbsfjw.html

[R42] 输入重定向
来源：http://hz.tanke756.top/gtgyslipqz.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtrgreyiuo.html

[R43] 按名字查找文件
来源：http://hz.cucudq.cn/gtzuvqduak.html

find . -name "*.log" -type f
来源：http://hz.aibaodan.cn/gtlkafxlbm.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtbauotbab.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtxgbfayhk.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtlpowvigf.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gtgzkxrhgk.html

[R46] 递归替换文件内容
来源：http://hz.jinyuanbaomall.cn/gtmtoyqhhk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtenptnkfo.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtwziyhhsu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtbbgtfmjb.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gtkklqhzed.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtfejwuvlt.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtyaprlpqb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.redwolf501.top/gtxjfvnrgc.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtubwvyftk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gthqlibkrn.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtftxgtios.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtkblhguic.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtbxmhidpa.html

wc -l a.txt
来源：http://hz.cashguo.top/gtqxksccbn.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gtplyphfyf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gtqrhragne.html

[R54] 比较两个文件
来源：http://hz.jlsjyb.cn/gtcadrcouu.html

diff a.txt b.txt
来源：http://hz.daria6918.cn/gtoiskeplb.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtjmmljefp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.birdmap.top/gtqgsphlij.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtfnhhkbfa.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtrdscyscu.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtmhspcika.html

ssh user@host 'uptime'
来源：http://hz.kuanghao11.cn/gtbkjnnueg.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtkmpkdmnm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hysaishi.cn/gtftmvhspf.html

[R59] 发 POST JSON
来源：http://hz.feifeiyinyue.top/gtjarojyju.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gterkzhjjt.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtbqhvdcxa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtspynzcug.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtxttpmohx.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtnqcdgmnt.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtzkdtyscg.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtzrfxwaqh.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtdgbsqmjw.html

free -h;  ps aux | grep nginx
来源：http://hz.havefunace.top/gtiyeyxvib.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtwpuqtvpa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtjdntruen.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtkogrozji.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtnttzqols.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gttvghvwvu.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gtdevinemc.html

[R67] 生成随机十六进制串
来源：http://hz.yuanzhike.top/gtpdvgzpgd.html

openssl rand -hex 16
来源：http://hz.jinqigufen.top/gtnuzwazhk.html

[R68] 计算文件校验值
来源：http://hz.ppjwa.cn/gtngvkwpdr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ehwqpu.com/gtpjyakavt.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtbapxhgyr.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtenkuvvue.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gtxlgxqvhs.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtfneweifc.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtadlxcpcq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shuidangran.top/gthypysxka.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtwsqnkowy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtfrokhter.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtnodidybz.html

split -l 1000 big.log part_
来源：http://hz.vqdsnc.cn/gtbaxvkzjs.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtxwrtyuyc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtcrpmwefe.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtnrvqdwwj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhengqikj.top/gtavrdnndp.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtxwdopczi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtiuahpdaw.html

[R77] 读取用户输入
来源：http://hz.meibo888.top/gtofveuqaq.html

read -rp "请输入: " ans
来源：http://hz.gogol.net.cn/gttpszyjrc.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gtfdhxttsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gtzvycohgq.html

[R79] 解析命令行选项
来源：http://hz.yangfankeji.com/gtnfmkelwv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtlizattxy.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtcguwlkfj.html

time ./run.sh
来源：http://hz.c1oappe.top/gtzmqssias.html

================================================================================
来源：http://hz.jianghu66.top/gtmwaeatuq.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtcnrljfya.html

================================================================================
来源：http://hz.zycfv.cn/gtxccuuuus.html

[S01] C：Hello World
来源：http://hz.guowangkeji.top/gtolmgwcaa.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gtragjvqyh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtichndkph.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gtxhmkwdhs.html

int a = 10; printf("%d\n", a);
来源：http://hz.hfpthk.cn/gtycruolrc.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtahgvbobb.html

int x; scanf("%d", &x);
来源：http://hz.zhijiandao.cn/gtexmfdzxh.html

[S04] C：字符串复制
来源：http://hz.hnxiangtu.top/gteejhdgty.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtnkomwcaw.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtwaqrrgvy.html

strlen(s)
来源：http://hz.ydzc1.top/gtglzyxlqw.html

[S06] C：字符串比较
来源：http://hz.gzhubu.top/gtakdptnqc.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtjrnzzmvi.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtblfxaxbi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yueranfly.top/gtwmfkmhgt.html

[S08] C：动态内存分配与释放
来源：http://hz.zhoulong.xyz/gtvmhlboob.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtlcfyjupj.html

[S09] C：结构体定义与初始化
来源：http://hz.wangdashe.top/gtlfzzrdna.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.feifeiyinyue.top/gtfzrertkv.html

[S10] C：指针与解引用
来源：http://hz.jinyuanbaomall.cn/gtstjdfkse.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtpukjiucg.html

[S11] C：逐行读文件
来源：http://hz.dianchejie.cn/gtfbfxejxb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtxzlanmzf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yanxiufei.cn/gtwpbrirkn.html

fclose(f);
来源：http://hz.zhixingplan.top/gtofaufvsk.html

[S12] C：写文件
来源：http://hz.xingfuxueyuan.xyz/gthrfaqfrk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtdehphvig.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gttuiqodue.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtrwnsdimi.html

[S14] C：枚举
来源：http://hz.snrcjt.cn/gtnievcuwy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guowangkeji.top/gtpeqeupvz.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gtmjmliezg.html

(double) a / b
来源：http://hz.gzhubu.top/gtkzslowfp.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtekmrhstq.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtiwgdymjw.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtljiwtgmw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nwbrower.top/gtvzdymkrs.html

[S18] C：命令行参数
来源：http://hz.ppjwa.cn/gtwsyokhuw.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gtqafjfbwm.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gteijytvzq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtiahwyyrs.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtgfgbjwgd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtvyqtwgae.html

[S21] C：字符类别判断
来源：http://hz.dianchejie.cn/gtfumbhqlj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtrvrxrnpa.html

[S22] C：字符串转数字
来源：http://hz.hywenlv.cn/gthtgwopvz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinyuanbaomall.cn/gtwckmgjfa.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gtbvweoxfg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangtech.top/gtkbrzwttd.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gteykimfci.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtqtnqpzln.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtaqkfvxfh.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtxggikcqc.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtyyhmbwhw.html

memset(a, 0, sizeof a);
来源：http://hz.ppjwa.cn/gtziebbbrn.html

[S27] C：定义常量
来源：http://hz.chenjidiqi.icu/gtjxdnzqxi.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtpbkducny.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtylarhsxx.html

static int counter = 0;
来源：http://hz.xingfuxueyuan.xyz/gtkuexafeb.html

[S29] C：变参函数
来源：http://hz.hammf.cn/gtfzpuocot.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtkwjgqqmp.html

[S30] C：头文件保护
来源：http://hz.chenjidiqi.icu/gtzseftuhh.html

#ifndef X_H
来源：http://hz.yueranfly.top/gtyhsyxakd.html

#define X_H
来源：http://hz.gzhubu.top/gtgiqgibjs.html

#endif
来源：http://hz.sysykeji.top/gtldmffwiu.html

[S31] C++：Hello World
来源：http://hz.hnxiangtu.top/gtdzbkmgry.html

#include <iostream>
来源：http://hz.zdqjudy.top/gtbmnfkwoi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtvmkpjdpz.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gtmqsazesc.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtwzazamqm.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtnpkqcrjb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinyuanbaomall.cn/gtvqcobtvl.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtqoibgadc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtvwjanaqy.html

[S35] C++：map
来源：http://hz.ywan-chungtsiang.top/gtsjgdzjzz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtltrhxfro.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtogdiqtmv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtbkkxkjbb.html

[S37] C++：set
来源：http://hz.yj20258888.top/gtckyndqoe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sufxvd.cn/gttgydbwfl.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtzrlnuezv.html

std::sort(v.begin(), v.end());
来源：http://hz.jinghuilouyu.cn/gtdpbbdfpa.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtqulmbwgf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtansayvjz.html

[S40] C++：查找元素
来源：http://hz.xinyue.icu/gtzvgzgzxw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtogmerido.html

[S41] C++：类与构造函数
来源：http://hz.hammf.cn/gtaovlynqg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtardlhscq.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtqdugzywf.html

class B : public Base { public: void f() override {} };
来源：http://hz.jlsjyb.cn/gtlbbcobqn.html

[S43] C++：智能指针
来源：http://hz.shzxlz.cn/gtczoyqrnk.html

auto p = std::make_unique<int>(5);
来源：http://hz.xylfe.cn/gtkmvdqpdr.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gtwsrzsogv.html

void inc(int &x) { ++x; }
来源：http://hz.c1oappe.top/gtihyqqaye.html

[S45] C++：lambda
来源：http://hz.hammf.cn/gtjnlherxa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtjoidbcuj.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtphcqxund.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daria6918.cn/gtkzastuvj.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtszbjcubt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtqjhdjakj.html

[S48] C++：逐行读文件
来源：http://hz.jqgfzy.top/gtssjiwlaa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtfdktjtng.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gthewpkriv.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gtrylhqidd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtqjxboonu.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtrrkwktlv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtahbmazxx.html

[S51] C++：显式类型转换
来源：http://hz.c1oappe.top/gtdmycwrhv.html

static_cast<double>(a) / b
来源：http://hz.yongpay.top/gtbadeoxkd.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gttodjybdp.html

int size() const noexcept { return n_; }
来源：http://hz.sweek.top/gtcueaicay.html

[S53] C++：移动语义
来源：http://hz.zhijiandao.cn/gtfevagddt.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtwalrzyki.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gtgtjqzzcn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gthaoxgfwt.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtgnomepps.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangkeji.top/gtyjxjnoqu.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtblbpalzt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtdtxenvqt.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtporljjpi.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gtwtmxqsim.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtoaszaxse.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gtzmdejhpe.html

[S59] C++：静态断言
来源：http://hz.yueranfly.top/gtldjprmlr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daxiang520.top/gtjvtdfkxt.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgfzy.top/gtbcqgbdgx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtijbxtjcb.html

================================================================================
来源：http://hz.smart0.xyz/gtbfisymdv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtrdxejaev.html

================================================================================
来源：http://hz.cdnleiting.top/gtzumkdcca.html

[T01] Kotlin：Hello World
来源：http://hz.meibo888.top/gtpnngqehc.html

println("Hello")
来源：http://hz.cheryme.top/gtjbkdpqud.html

[T02] Kotlin：变量
来源：http://hz.nanxinkj.top/gtjqsxrfjz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtsbbbxryx.html

[T03] Kotlin：字符串模板
来源：http://hz.guowangkeji.top/gtlvqpnmaa.html

"值: $b"
来源：http://hz.chenlongwang.top/gtrrptxrnw.html

[T04] Kotlin：空安全
来源：http://hz.xuanzx.com/gtbphsawyg.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtyeafgonk.html

[T05] Kotlin：when 表达式
来源：http://hz.ywan-chungtsiang.top/gtdtqzfczo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gthslmcmju.html

[T06] Kotlin：集合映射
来源：http://hz.chenjidiqi.icu/gtqvojmexz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhaomingkeji.xyz/gtzjseqpyy.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258888.top/gtocipqdac.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gtswvbgazc.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gteyutuvha.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangtech.top/gtbxoqtdbd.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtccexhzes.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtxhykspll.html

[T10] Kotlin：默认参数
来源：http://hz.cashguo.top/gtwaezztjm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pengpengdd.cyou/gtqmuxhcwl.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtgkomuxau.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtbuawfwlv.html

[T12] Kotlin：解构声明
来源：http://hz.tanke756.top/gtinbcjetu.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtnimijyow.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtbfdctvsv.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtpimryrul.html

[T14] Kotlin：循环
来源：http://hz.redwolf501.top/gtaljnblyd.html

for (i in 1..10) println(i)
来源：http://hz.dashuyun.cn/gtvjtzkydz.html

[T15] Kotlin：接口
来源：http://hz.guowangkeji.top/gtbhhcmedw.html

interface Shape { fun area(): Double }
来源：http://hz.jianghu66.top/gttubncfsz.html

[T16] Swift：Hello World
来源：http://hz.tianlin.xyz/gtlaqxgwle.html

print("Hello")
来源：http://hz.fzhhl.top/gtwhonkrqb.html

[T17] Swift：变量与常量
来源：http://hz.wangdashe.top/gtxictrprd.html

var a = 1;  let b = 2
来源：http://hz.hywenlv.cn/gtykopvqsp.html

[T18] Swift：字符串插值
来源：http://hz.chenzaomai.com/gtxyoqmklu.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gtwayqxfzh.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtmitjgpgz.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtjcjlncid.html

[T20] Swift：数组操作
来源：http://hz.hfpthk.cn/gtuqivrrbn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuanzhike.top/gtdsddyzix.html


<!-- 参考信息 -->