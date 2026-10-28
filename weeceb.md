代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gogol.net.cn/gtwtonzsqx.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtetpymnff.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtjbgmdumu.html

[R17] 数组定义与取值
来源：http://hz.hongshengwenyu.top/gtciymlcce.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtwnvagcgc.html

[R18] 遍历数组
来源：http://hz.mhx1999.top/gtyxhsvlgj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aizwys.cn/gtgyztgbiv.html

[R19] 数组长度
来源：http://hz.aibaodan.cn/gteobtinmi.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtsoatyrxk.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gtnwnjawcs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtmrknpqxb.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtqogrxlcr.html

echo "${#s}"
来源：http://hz.gaohongyu789.top/gtpliyuuei.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtcfmhewth.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtohtutgku.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtoozklxyw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtvmocqysd.html

[R24] 大小写转换
来源：http://hz.yvedp.cn/gtulnkrgxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gteixasowh.html

[R25] 去后缀 / 去前缀
来源：http://hz.gotoacloud.top/gtbeytgpop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gtuegtgaxw.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtwnutkwuk.html

now=$(date +%F); echo "$now"
来源：http://hz.daxiang520.top/gtlyyqgywl.html

[R27] 算术展开
来源：http://hz.xuanzx.com/gtvemijitv.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtatiudcot.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtqljrstcg.html

echo "scale=2; 10/3" | bc
来源：http://hz.xziqi.cn/gtrewsiygz.html

[R29] 定义函数
来源：http://hz.pengpengdd.cyou/gtcmkxwzxa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtkbuqaglx.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtwufczfgk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtddclqjsm.html

[R31] 局部变量
来源：http://hz.nwbrower.top/gtiawzqnef.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinyuanbaomall.cn/gtdimvitkh.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtabqjqdll.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtezgyfxmz.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258.top/gtfcqhiszd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtbqlhcmfq.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtlusocsgj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtjhhqdcsb.html

[R35] 后台执行并等待
来源：http://hz.feifeiyinyue.top/gtyadnsxvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtyinzhlyj.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtjhvifnjd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtvgbxdovf.html

[R37] 把输出赋给变量
来源：http://hz.fengsongda.top/gtfwnoryoo.html

files=$(ls -1)
来源：http://hz.xylfe.cn/gteotsgzpx.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtcjdwpkuf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ywan-chungtsiang.top/gtikwvdcqu.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtzvvuhifb.html

cmd > out.log 2>&1
来源：http://hz.iojbl.cn/gthfgjqbok.html

[R40] 追加写日志
来源：http://hz.shanyushiyangkeji.top/gtfphbdduc.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtcimqonlj.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gtpycnbgsu.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtqqaknrhs.html

[R42] 输入重定向
来源：http://hz.hysaishi.cn/gtwsxmyoyl.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtippsljxq.html

[R43] 按名字查找文件
来源：http://hz.zhiwuduotai.top/gtpbdnfhxl.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtwdvkkxoy.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtclzmfsos.html

find . -mtime -7 -type f
来源：http://hz.yangfankeji.com/gtkskifcrb.html

[R45] 批量删除
来源：http://hz.jqgfzy.top/gtnygiersn.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtklmzqpka.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtpaohfwmp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtqojzozxt.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtdqxvtqie.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtfyjrxbvg.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtlmkzxrdl.html

awk '{print $1, $3}' a.txt
来源：http://hz.tanke756.top/gtofbwaozt.html

[R49] awk 带条件
来源：http://hz.ehwqpu.com/gtsottltoc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtztospfya.html

[R50] awk 求和
来源：http://hz.hongshengwenyu.top/gtlvfjqwnx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtnhfwlqjp.html

[R51] 排序去重取前几
来源：http://hz.zhaomingkeji.xyz/gtckxpxawb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtevtyauqr.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtwtinbnua.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtxzbritje.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtlnrivpck.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtiossgiys.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtppvfdnpp.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gtxxuclwzq.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtkywcqpwj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuxming.cn/gtrmbtwsai.html

[R56] 远程拷贝
来源：http://hz.xylfe.cn/gtmdvpwzdg.html

scp file user@host:/path/
来源：http://hz.redwolf501.top/gttboinlfd.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtafcqxuns.html

ssh user@host 'uptime'
来源：http://hz.hongshengwenyu.top/gtwquuzcpr.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtunuxrsoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenlongwang.top/gtlrhfzjmb.html

[R59] 发 POST JSON
来源：http://hz.yangfankeji.com/gtszlmrbnp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenjidiqi.icu/gtnqylhsia.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnqzz.top/gtovcrlwyj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuanzhike.top/gtfrxlkwqf.html

[R61] 磁盘占用
来源：http://hz.cqqwz.cn/gtfnrjcovz.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtupmmfroz.html

[R62] 找最占空间的文件
来源：http://hz.xinyue.icu/gthxkpnadj.html

du -ah . | sort -rh | head -10
来源：http://hz.jinghuilouyu.cn/gtvneeeafd.html

[R63] 内存与进程
来源：http://hz.ppjwa.cn/gtztrpzflk.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtubpjizds.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtrppegrki.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gtjesvacnb.html

[R65] 查看端口占用
来源：http://hz.zhoulong.xyz/gtqxpzjtuc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj202588.top/gtfjzykcza.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtcfrekyvp.html

crontab -e;  crontab -l
来源：http://hz.hongshengwenyu.top/gtzokxifis.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtekuefjfc.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtxhfrgkkh.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtizwtrkyl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtzrtuclyl.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtmjsgunyn.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtykocnmys.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtfnuidvbm.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtwahbgtqv.html

[R71] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtwoktiqff.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhengqikj.top/gtqezvavjz.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtycheixdy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtcdigavhl.html

[R73] 分割大日志
来源：http://hz.pycfn.com/gtmhsmmyej.html

split -l 1000 big.log part_
来源：http://hz.jyoumei.cn/gtmpkdggfo.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gttiloqpxp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtxshmxzke.html

[R75] 导出环境变量
来源：http://hz.jqgufenzy.top/gtehrqnwkn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtlgvrnrwa.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gtzgxvjmur.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtfujcvjgr.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gtnavlpfxv.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gthwqczhnm.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gtzyboynvd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtuokhozgj.html

[R79] 解析命令行选项
来源：http://hz.guannengcc.top/gtakfgzqpd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gzhubu.top/gtolikcnqc.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtwsbcihsx.html

time ./run.sh
来源：http://hz.zhiwuduotai.top/gtfcokqzem.html

================================================================================
来源：http://hz.gzhubu.top/gteaxzawou.html

S. C / C++ 专题
来源：http://hz.zhongyouzk.top/gtyiukdthl.html

================================================================================
来源：http://hz.yj20258888.top/gtedqlwwsa.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtirdwhubr.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtzshikamd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydjk.org.cn/gtoqcrpqzy.html

[S02] C：变量与格式化输出
来源：http://hz.snrcjt.cn/gtacpndgor.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtxapiqdhs.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gtypratatg.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtwjvolaio.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtstdrnwdv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gtujslnrod.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtekorpksr.html

strlen(s)
来源：http://hz.zhaomingkeji.xyz/gtfhuxxjjq.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtdizfpadg.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtxvgmheea.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gtvzcrqppp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ehwqpu.com/gtcpytceqh.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtwhqcapaw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtjzamwgul.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtbfozjlcm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zycfv.cn/gtzotziocw.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gthitpsyqh.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtqpugdiiv.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtylqrjlxg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtnvdokasb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gttnlulkuz.html

fclose(f);
来源：http://hz.shuidangran.top/gteyekfcms.html

[S12] C：写文件
来源：http://hz.dashuyun.cn/gtwnsrosqx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aizwys.cn/gtnwwpjtrn.html

[S13] C：宏定义
来源：http://hz.yueranfly.top/gtekvevibh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.smart0.xyz/gtkysxhrxo.html

[S14] C：枚举
来源：http://hz.jinyuanbaomall.cn/gttupzfeax.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuxming.cn/gtweciieis.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtcnkuptgj.html

(double) a / b
来源：http://hz.0kj1m.cn/gtlfygrdmr.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gthsowgwji.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtecyrfzhr.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtebqaapal.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhiwuduotai.top/gtgjzscmwk.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtlvbjuywg.html

int main(int argc, char **argv)
来源：http://hz.ehwqpu.com/gtsaraatrt.html

[S19] C：快速排序
来源：http://hz.zhixingplan.top/gtwieqbqsj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtrylqvcdl.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtdsrayemb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtxyprqolm.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtcsuqjevl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nwbrower.top/gtlzbzgnmj.html

[S22] C：字符串转数字
来源：http://hz.wangshuangyany.cn/gtddmysjea.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtldztxxcs.html

[S23] C：随机数
来源：http://hz.jinqigfzy.top/gteyyzkxfs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.0kj1m.cn/gtxpvyxddc.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtwrjdgasf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zdqjudy.top/gtausqujdx.html

[S25] C：内存拷贝
来源：http://hz.hysaishi.cn/gtikvcylmz.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtdgnjprpk.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtdidhpgzi.html

memset(a, 0, sizeof a);
来源：http://hz.gaohongyu789.top/gtczaquywk.html

[S27] C：定义常量
来源：http://hz.jinyuanbaomall.cn/gtxfdschqj.html

const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtqqovncxw.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtypczquut.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtsyimoqxy.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtjsaopvya.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtoiglyfts.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtmmkrbzzy.html

#ifndef X_H
来源：http://hz.cashguo.top/gtxfklvwas.html

#define X_H
来源：http://hz.fengsongda.top/gttlepwuwt.html

#endif
来源：http://hz.ydjk.org.cn/gtxxrlhnyk.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtuqidroev.html

#include <iostream>
来源：http://hz.yuxming.cn/gtxaqjniva.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtevfbtywe.html

[S32] C++：字符串
来源：http://hz.yonumen.top/gtvmjczpne.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtupunrimt.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtcpipvncd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtadquzhtb.html

[S34] C++：遍历 vector
来源：http://hz.tian-w.cn/gteesjvxfs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtmsuyzeiy.html

[S35] C++：map
来源：http://hz.wangdashe.top/gtqzfwysdw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtqszyhuhr.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gthvxunvlz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtmjuofoyq.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtcfunxytf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtkivboxrs.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gtpuowfhsm.html

std::sort(v.begin(), v.end());
来源：http://hz.pycfn.com/gtijmamcqm.html

[S39] C++：自定义比较器排序
来源：http://hz.yanxiufei.cn/gtxvbsdlej.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gtpnvtaanf.html

[S40] C++：查找元素
来源：http://hz.cashguo.top/gtedomhacc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtbdiykydp.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtwtkcnmyw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangdashe.top/gtxhwqgauz.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtuftrhzjm.html

class B : public Base { public: void f() override {} };
来源：http://hz.ppjwa.cn/gtcecynngs.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtbsfcqtem.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gttvrnsapw.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gteicxbilb.html

void inc(int &x) { ++x; }
来源：http://hz.gzhubu.top/gtoriyfpde.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtitvofrra.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtqrevyiqt.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtgsiuyyhh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtplmliakp.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtyvwugfym.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtmevwtmoy.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtunvbvvym.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtospafilj.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtqufhstxm.html

[S49] C++：写文件
来源：http://hz.tianlin.xyz/gtxjusizhm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtltzhpvqz.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtjulvbdgo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gttvhlvrzp.html

[S51] C++：显式类型转换
来源：http://hz.jinghuilouyu.cn/gtlagoflcx.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gthiqepxap.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gthxrqqygw.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtalvnmonu.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gtmqqlqwpu.html

std::vector<int> w = std::move(v);
来源：http://hz.yuxming.cn/gtblbhbyin.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gtuzmpowcp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtrvaxkffj.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtzmouzkcw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtxtrktetp.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtxblxmuqh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtuvxdabth.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtdtsmzqyq.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtmqwlcvrg.html

[S58] C++：命名空间
来源：http://hz.yonumen.top/gtamrbyxwa.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtxpsochdw.html

[S59] C++：静态断言
来源：http://hz.jinyuanbaomall.cn/gtbvwkolxa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtfjwfuflv.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtynkqddze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtykivgkek.html

================================================================================
来源：http://hz.chenzaomai.com/gtrmejbcux.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtycywyrft.html

================================================================================
来源：http://hz.cheryme.top/gtyvprehtz.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gthhxujlfw.html

println("Hello")
来源：http://hz.shuidangran.top/gtqilfkxwr.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtjsggebgb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtnemcfwce.html

[T03] Kotlin：字符串模板
来源：http://hz.cqqwz.cn/gtqngvjudw.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gttrubeebt.html

[T04] Kotlin：空安全
来源：http://hz.xuetiantiany.cn/gttcapunfw.html

val n: String? = null;  n?.length
来源：http://hz.nanxinkj.top/gtweiapttk.html

[T05] Kotlin：when 表达式
来源：http://hz.ydjk.org.cn/gtopljjsze.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtohnazcbr.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtaullhens.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.feifeiyinyue.top/gtnrimldpz.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtztoysywm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gaohongyu789.top/gtzllofgoi.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtdkzcesgs.html

data class User(val name: String, val age: Int)
来源：http://hz.mhx1999.top/gtakzklklr.html

[T09] Kotlin：扩展函数
来源：http://hz.meibo888.top/gtctqtyujp.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gterdpfezq.html

[T10] Kotlin：默认参数
来源：http://hz.c1oappe.top/gttghfepnn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gtzaccryck.html

[T11] Kotlin：协程
来源：http://hz.ywan-chungtsiang.top/gtmqnzqlul.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.mhx1999.top/gtyatlrodv.html

[T12] Kotlin：解构声明
来源：http://hz.yuxming.cn/gtwurvfiph.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gtechtrujn.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigfzy.top/gtstgqpcba.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gtsnbcizbu.html

[T14] Kotlin：循环
来源：http://hz.ywan-chungtsiang.top/gtwnaysovw.html

for (i in 1..10) println(i)
来源：http://hz.meibo888.top/gthaszgsoz.html

[T15] Kotlin：接口
来源：http://hz.yongpay.top/gtlelerple.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtuxwpkrop.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtsvyijwpd.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtusoifeds.html

[T17] Swift：变量与常量
来源：http://hz.smart0.xyz/gtjquipyrg.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtqftluxtl.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtxyfugywh.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gttxmulkpj.html


<!-- 参考信息 -->