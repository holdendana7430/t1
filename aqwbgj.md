代发 wailian999

esac
来源：http://hz.havefunace.top/gtcsynhjtw.html

[R12] for 遍历文件
来源：http://hz.gaohongyu789.top/gtgdvqzpmy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gtgrunfpjj.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtzufnadwv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jiagoushi.top/gttvxftquy.html

[R14] C 风格 for
来源：http://hz.shangyingyoupin.top/gtsrotolwi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtjkepbdfj.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtskzcysxz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.snrcjt.cn/gtmaalstxo.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtcgorhayg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gtwvzxldty.html

[R17] 数组定义与取值
来源：http://hz.chenzaomai.com/gtdbkbgljb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtoeturkag.html

[R18] 遍历数组
来源：http://hz.feifeiyinyue.top/gtypfhbrig.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtewjjiodj.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtcmkgfhbb.html

echo "${#arr[@]}"
来源：http://hz.aizwys.cn/gttwjcsdbr.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtvykosnlr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtqzsrxdqt.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtotjhevow.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtoddhgpvw.html

[R22] 截取子串
来源：http://hz.tanke756.top/gtpxquepvl.html

echo "${s:0:5}"
来源：http://hz.jinqigufen.top/gtzwlqylny.html

[R23] 字符串替换
来源：http://hz.hnxiangtu.top/gtmlswdebp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenlongwang.top/gtcbdnmqmk.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtgvwxqqkr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtlsjubjdf.html

[R25] 去后缀 / 去前缀
来源：http://hz.zdqjudy.top/gtiaxbeufq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.andypj.xyz/gtliqmunfj.html

[R26] 命令替换
来源：http://hz.yonumen.top/gtbejrqrtc.html

now=$(date +%F); echo "$now"
来源：http://hz.sweek.top/gteojxdjpy.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtbtinvqcv.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtpeqkrbbt.html

[R28] 浮点运算
来源：http://hz.shzxlz.cn/gtxeowkmku.html

echo "scale=2; 10/3" | bc
来源：http://hz.jlsjyb.cn/gtlsylcffe.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtjeqqfqlq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gthkdivcxs.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtdckhbden.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtembyfkbj.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtkoypdtxh.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhongyouzk.top/gtuyzdqtdz.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gttpsstcrw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtriouzbls.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gttsbxqhek.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtkfffcbpa.html

[R34] 退出时清理
来源：http://hz.chenjidiqi.icu/gtnlqusjsk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtdqtqafxw.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtxjqxfsqq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yanxiufei.cn/gtgropxjbg.html

[R36] 并发执行多个任务
来源：http://hz.sysykeji.top/gtkzfnagpi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtoirejvdr.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtsifmhxit.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtetqbygxf.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gtwbqplgnv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jianghu66.top/gtfiqufdaf.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtltpmnyex.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtswwosqol.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtnttomyxs.html

echo "log" >> out.log
来源：http://hz.c1oappe.top/gtkfpgaccc.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtiewksqsx.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtwakqzbkp.html

[R42] 输入重定向
来源：http://hz.sweek.top/gtrttlklmz.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtynzzxano.html

[R43] 按名字查找文件
来源：http://hz.sxryk.cn/gtbtlztjhv.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtecwajhez.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gthjlyhybc.html

find . -mtime -7 -type f
来源：http://hz.zhaomingkeji.xyz/gtcupqhpdf.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtokirwxcq.html

find . -name "*.tmp" -delete
来源：http://hz.ybcxt.top/gtptsqwlxa.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtnrsockmm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtqcxtcqlx.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gthxqrjxiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sxryk.cn/gthfdjrcdo.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtnxponroq.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtorvlvagm.html

[R49] awk 带条件
来源：http://hz.gaohongyu789.top/gtnjfltinn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sweek.top/gtyuqdevlq.html

[R50] awk 求和
来源：http://hz.zhixingplan.top/gtvffcbuyj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtptphdajy.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gtabfurdom.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhongyouzk.top/gthvatqwmc.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gtrofqkcet.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtjgdzpxes.html

[R53] 查看文件头与实时尾
来源：http://hz.havefunace.top/gtlwkkxilf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtvcpitjsf.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gtoqkvzgth.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtuuxzdiwj.html

[R55] 压缩与解压
来源：http://hz.fengsongda.top/gtjuzjetcz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tian-w.cn/gtavacnjkr.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtxthprzwi.html

scp file user@host:/path/
来源：http://hz.nanxinkj.top/gtgvwbofoo.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gtvluhvrnm.html

ssh user@host 'uptime'
来源：http://hz.yonumen.top/gthuuthcyf.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtzsuzltdr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xziqi.cn/gtdlsuuiwq.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gtopcgzxmv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gtxllvukoa.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtkirgfged.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtxzfsctoq.html

[R61] 磁盘占用
来源：http://hz.nanxuanxn.top/gtictxyixm.html

df -h;  du -sh *
来源：http://hz.yj202588.top/gtoybjgvmg.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtauhbgnjr.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtnjssqaxl.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtzjcfmuqo.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtocgboosl.html

[R64] 结束进程
来源：http://hz.snrcjt.cn/gtnubpdfdw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtcdtqbikf.html

[R65] 查看端口占用
来源：http://hz.cheryme.top/gtmrsyfcrq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtlpubcnof.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtkqhzfuxq.html

crontab -e;  crontab -l
来源：http://hz.yangfankeji.com/gtrucqbfix.html

[R67] 生成随机十六进制串
来源：http://hz.fengsongda.top/gtoycnczwg.html

openssl rand -hex 16
来源：http://hz.vqdsnc.cn/gtsxbkgoff.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtcsynngls.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gthcuzlcsm.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gtwwsvvvgn.html

head -c 16 /dev/urandom | base64
来源：http://hz.snrcjt.cn/gtjzqjlwfk.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtsnciqpzy.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtycvjynbf.html

[R71] 日期格式化
来源：http://hz.cqqwz.cn/gtizgueoco.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gthycqpuko.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtnavgvezy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenzaomai.com/gtzwgqicwz.html

[R73] 分割大日志
来源：http://hz.sxryk.cn/gtgsquwzyw.html

split -l 1000 big.log part_
来源：http://hz.9152youxi.cn/gtttictteb.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtpqhoeyjx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtxkghveaw.html

[R75] 导出环境变量
来源：http://hz.nanxuanxn.top/gtxhzuohxp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxuanxn.top/gtnlgvmzkv.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gthplctkdl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtxkkxundt.html

[R77] 读取用户输入
来源：http://hz.daria6918.cn/gtmsbgxrei.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gtwhxwetwl.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtkmekzvqj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gtbabvkahn.html

[R79] 解析命令行选项
来源：http://hz.hfpthk.cn/gtmuntvpgy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtwvvhcntv.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gttchynscw.html

time ./run.sh
来源：http://hz.redwolf501.top/gtgpifvowo.html

================================================================================
来源：http://hz.yonumen.top/gtxmjlryje.html

S. C / C++ 专题
来源：http://hz.zhoulong.xyz/gtmqwwflkm.html

================================================================================
来源：http://hz.c1oappe.top/gtvrtadeoa.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtxfpuaizu.html

#include <stdio.h>
来源：http://hz.gaohongyu789.top/gtnxxmniuk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtgddmfetj.html

[S02] C：变量与格式化输出
来源：http://hz.nanxuanxn.top/gtqxqxsjqc.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gtqujlnehd.html

[S03] C：读入整数
来源：http://hz.snrcjt.cn/gtyjncvqso.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gtsaepjbya.html

[S04] C：字符串复制
来源：http://hz.shuidangran.top/gtrfcfvqmz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sufxvd.cn/gtnkohjbho.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtynweibee.html

strlen(s)
来源：http://hz.zycfv.cn/gtndbuzcqh.html

[S06] C：字符串比较
来源：http://hz.jlsjyb.cn/gtkomfpuqm.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtyxzzuqxy.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtnqyzvvbw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gtzkekpzrl.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtvbencnik.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gthgslhgmr.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtzwwaoary.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangkeji.top/gtlxuwluuv.html

[S10] C：指针与解引用
来源：http://hz.zhijiandao.cn/gtjnctvyus.html

int *p = &a;  *p = 5;
来源：http://hz.yanxiufei.cn/gtsvuhnnqm.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gtvbuiovke.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.52xcode.cn/gthwluhojg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zdqjudy.top/gtjjirhodo.html

fclose(f);
来源：http://hz.yj20258.top/gtvdafmbit.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtbsgjabqy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.vqdsnc.cn/gtsbuwxfcg.html

[S13] C：宏定义
来源：http://hz.jianghu66.top/gttsqvzpdh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtafiocmbu.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gttwcbmsvr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtxeywmjdg.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtndtgulop.html

(double) a / b
来源：http://hz.yongpay.top/gthoyinrdy.html

[S16] C：位操作置位
来源：http://hz.cheryme.top/gtbldruvwb.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtniowbegs.html

[S17] C：安全拼接字符串
来源：http://hz.gogol.net.cn/gtywdrbheu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtsgvokwex.html

[S18] C：命令行参数
来源：http://hz.yj20258888.top/gtupwotoom.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtgxzshccm.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtuimodhzj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtnfyvpgye.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gtaaewcsbb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtesbkmlld.html

[S21] C：字符类别判断
来源：http://hz.316326.xyz/gtjkojksmy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fzhhl.top/gtyyfduofs.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtlxgckgfd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgfzy.top/gtjktbcmch.html

[S23] C：随机数
来源：http://hz.aizwys.cn/gttjnvcnzt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangtech.top/gtuahxekul.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtawmkejgv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hysaishi.cn/gtheezgudt.html

[S25] C：内存拷贝
来源：http://hz.feifeiyinyue.top/gtbabufwap.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gtcofmenjo.html

[S26] C：内存清零
来源：http://hz.meibo888.top/gtrejwznpd.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gtoehmcsdr.html

[S27] C：定义常量
来源：http://hz.cashguo.top/gtwjtnjivr.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtwjsqehon.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtdflkomyf.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gtaufywose.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtycybxnni.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.haohaochexian.top/gtfgwdrniw.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtvyzperyl.html

#ifndef X_H
来源：http://hz.shangyingyoupin.top/gtwxclfqtb.html

#define X_H
来源：http://hz.jinghuilouyu.cn/gtuyfsckyd.html

#endif
来源：http://hz.sxryk.cn/gtlaybfaxj.html

[S31] C++：Hello World
来源：http://hz.bjfxy.top/gtgpbumjfo.html

#include <iostream>
来源：http://hz.tanke756.top/gtegfbfgzc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtmpcibqza.html

[S32] C++：字符串
来源：http://hz.daria6918.cn/gtavqyicqb.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtmcqclyvq.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtuemqwcfv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenjidiqi.icu/gtjbrlhhqq.html

[S34] C++：遍历 vector
来源：http://hz.nwbrower.top/gtzpiaoukh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhixingplan.top/gtypsogzlc.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtoznedfdo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtffyyysez.html

[S36] C++：unordered_map
来源：http://hz.zhoulong.xyz/gteqkgvncj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtxbdlyzty.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtdaylppcd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hongshengwenyu.top/gtqrlzoawf.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtpnmcwpfb.html

std::sort(v.begin(), v.end());
来源：http://hz.cashguo.top/gtudmyrlzt.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtrricrcrj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtzibqqhqi.html

[S40] C++：查找元素
来源：http://hz.mhx1999.top/gtavieoppd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtemouwknn.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtsjjwhlvk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtkktcocfd.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtubetwfss.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhaomingkeji.xyz/gtszibprvi.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtwtibjqdh.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtdunjegup.html

[S44] C++：引用传参
来源：http://hz.daxiang520.top/gtxtiuojwy.html

void inc(int &x) { ++x; }
来源：http://hz.quarkkingdee.top/gtgeapjsyv.html

[S45] C++：lambda
来源：http://hz.chenzaomai.com/gtdkvulowo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dianchejie.cn/gtkqvvorpx.html

[S46] C++：函数模板
来源：http://hz.chenjidiqi.icu/gtwmopnhyg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gtnovgemqo.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtrtllpvcw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtzvmzhtft.html

[S48] C++：逐行读文件
来源：http://hz.xylfe.cn/gtkkolkhtp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gteoaqdaxj.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtikoyisvr.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtxdujjyef.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtjxezofzz.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtxuwdnssl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtyfsxavdv.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gtlclewnpv.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtmldbpgxs.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtsbhtagft.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigufen.top/gthgazhxrg.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtdcbuqwxe.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtsustvmgy.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gtogvlruiu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xylfe.cn/gtoggjkdno.html

[S55] C++：结构化绑定
来源：http://hz.fzhhl.top/gtzmejqbhu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gttycvxkfa.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gtmhuhdrjf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daxiang520.top/gtjtqwokrr.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtjdohkxjr.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtrubttdkm.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtegeppyxl.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtzyerqzsi.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtfgmgucek.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gtfgvkxlvc.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtfvmkdpxg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtocvanheu.html

================================================================================
来源：http://hz.andypj.xyz/gtpdwapwzj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yongpay.top/gtejyluvwx.html

================================================================================
来源：http://hz.nanxinkj.top/gtabtkgzzb.html

[T01] Kotlin：Hello World
来源：http://hz.tian-w.cn/gtrjpnxggk.html

println("Hello")
来源：http://hz.zdqjudy.top/gtukveeflz.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gtlyiqkgzy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtozcdgaow.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gtfmgbnafj.html

"值: $b"
来源：http://hz.chenlongwang.top/gtqqisgmmj.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gthjujzdbj.html

val n: String? = null;  n?.length
来源：http://hz.meibo888.top/gtajgrejut.html

[T05] Kotlin：when 表达式
来源：http://hz.yuxming.cn/gtxnknpouw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtjsgdpuzg.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtvekmhusg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.kuanghao11.cn/gtvskdutla.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gthhsjayur.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gtpraioaug.html

[T08] Kotlin：数据类
来源：http://hz.yj202588.top/gtgzukbcsr.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtonkrzlte.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtrbgwhgxr.html

fun String.exclaim() = this + "!"
来源：http://hz.ydzc1.top/gtkwsvsusx.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gttwyekpyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gttwkbpnok.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtlqbdtsez.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ywan-chungtsiang.top/gtrrkanltk.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtkbazadvh.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangtech.top/gtbtiiudjq.html

[T13] Kotlin：只读 Map
来源：http://hz.bjfxy.top/gtlraiadqw.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtooqvtqkt.html

[T14] Kotlin：循环
来源：http://hz.hnxiangtu.top/gtvqwbdset.html

for (i in 1..10) println(i)
来源：http://hz.hywenlv.cn/gtnulpearz.html


<!-- 参考信息 -->