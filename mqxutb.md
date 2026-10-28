代发 wailian999

case "$1" in
来源：http://hz.hammf.cn/gtgxknxbwk.html

start) echo "启动" ;;
来源：http://hz.jqgfzy.top/gttzaznvju.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtrozerlqs.html

*)     echo "未知命令" ;;
来源：http://hz.ywan-chungtsiang.top/gtyjqxzaax.html

esac
来源：http://hz.xinyue.icu/gtymfqgtdv.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtndwrndvm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.bjfxy.top/gtfrjcogyv.html

[R13] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtfanuvfsp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtqrzabuhc.html

[R14] C 风格 for
来源：http://hz.fzhhl.top/gtfxconhiz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cucudq.cn/gtgslmfqan.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtpqwaklbk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtnymqqqut.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtxwwyuanx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gtvaymncpe.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gteqosoicn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gthipeerfm.html

[R18] 遍历数组
来源：http://hz.316326.xyz/gtrythdeov.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtbclrusof.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtneaxitpf.html

echo "${#arr[@]}"
来源：http://hz.wangshuangyany.cn/gtckflccum.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtpfodsfgz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtlbpesawe.html

[R21] 字符串长度
来源：http://hz.redwolf501.top/gtnnnionfx.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtwcpmvxeb.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gtuojbmspj.html

echo "${s:0:5}"
来源：http://hz.xylfe.cn/gttdxzelhu.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gtmoompzxi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xylfe.cn/gtazherxzz.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtkxkpjizf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ivvv.top/gtdevwunzc.html

[R25] 去后缀 / 去前缀
来源：http://hz.xylfe.cn/gtoxyqgchc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangtech.top/gtnteqorcy.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtgqzhmdbt.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtpcvekfro.html

[R27] 算术展开
来源：http://hz.hnxiangtu.top/gtkygafunc.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtotvmbikk.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gteqrgkwgz.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtpjneonfr.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtzyqlqnpi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtbmiroqod.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtpxkfmvgu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gtypvtdvmv.html

[R31] 局部变量
来源：http://hz.ehwqpu.com/gtvtbzthgz.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtbvlzoxwg.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtntnoivwi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnqzz.top/gtkhmhtgcc.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtdgzzdwyl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtlntjbcoj.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtlthokxjw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gteaemehjx.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gtwpziirzi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtluzniapc.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gtubewgpsj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtzbmeysgf.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtpgloezwk.html

files=$(ls -1)
来源：http://hz.cdnleiting.top/gttcrkmtlx.html

[R38] 管道串联
来源：http://hz.guowangkeji.top/gtoeafjqmk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zycfv.cn/gtkqxzklhs.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtumrmrfbc.html

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gttehqrsvf.html

[R40] 追加写日志
来源：http://hz.hnqzz.top/gtfuxpubal.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtxdepqbmi.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gtiallhric.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gthalyimwf.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtfizqgpur.html

wc -l < a.txt
来源：http://hz.hysaishi.cn/gtewxafyka.html

[R43] 按名字查找文件
来源：http://hz.chenzaomai.com/gtihyoayct.html

find . -name "*.log" -type f
来源：http://hz.gaohongyu789.top/gtknlqrlnp.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtkkygrdmz.html

find . -mtime -7 -type f
来源：http://hz.sysykeji.top/gtydakgibo.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtlprcvlef.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtarnjilqj.html

[R46] 递归替换文件内容
来源：http://hz.zhaomingkeji.xyz/gtvtrscovq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangtech.top/gtaalkcvpz.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gtczxumlui.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtarfzebuc.html

[R48] awk 取指定列
来源：http://hz.shuidangran.top/gtwioefiwq.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtzrediqjd.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtqretijqb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinghuilouyu.cn/gtasxluinz.html

[R50] awk 求和
来源：http://hz.andypj.xyz/gtmamdhbnn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtsqnifarl.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtvlpzcgrj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gtuxnicycl.html

[R52] 统计行数
来源：http://hz.hywenlv.cn/gtyabkazct.html

wc -l a.txt
来源：http://hz.c1oappe.top/gtspjygdky.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtmdwxvjtg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtygoxtxib.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtaqnbiwwt.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtsrdgbafv.html

[R55] 压缩与解压
来源：http://hz.sxryk.cn/gtbytmrlya.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gtcpbhbuwn.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtytwlcmxg.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtfhbtwrxl.html

[R57] 远程执行命令
来源：http://hz.gzhubu.top/gtuqcgngac.html

ssh user@host 'uptime'
来源：http://hz.daxiang520.top/gtvsemqxvc.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtwrviaezc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtqrepplfe.html

[R59] 发 POST JSON
来源：http://hz.sysykeji.top/gtmypccupp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cheryme.top/gtxgsqllsz.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtiiavekhl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtmldsggvf.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtejkacwgb.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtirzmjvvo.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gtssiezbrb.html

du -ah . | sort -rh | head -10
来源：http://hz.guowangkeji.top/gtscposngz.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtqkcvnujd.html

free -h;  ps aux | grep nginx
来源：http://hz.smart0.xyz/gtoeklfhdl.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtrkdspvhn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gtgtriqkab.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtvgixqnxd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtcphcjlrh.html

[R66] 定时任务
来源：http://hz.ydzc1.top/gtlmyaifoo.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtgenzdpyx.html

[R67] 生成随机十六进制串
来源：http://hz.zhoulong.xyz/gthkkfxgas.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtbhvkynbx.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtqmdpfglk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnxiangtu.top/gtrmqlgosb.html

[R69] 生成随机密码
来源：http://hz.sysykeji.top/gtxytbtslv.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtvowjvrhm.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtvnwggisf.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtclqcopwo.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtetxtfros.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtigevamxf.html

[R72] 等待端口就绪
来源：http://hz.chenlongwang.top/gtcfqkdrkz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtnitgjrqn.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gtptyjwelo.html

split -l 1000 big.log part_
来源：http://hz.jinqigfzy.top/gtrkqnkzjr.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtweavtpub.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtfdrfkwgf.html

[R75] 导出环境变量
来源：http://hz.yvedp.cn/gtrbgiqoit.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtyjfwuqya.html

[R76] 使用临时文件
来源：http://hz.9152youxi.cn/gtsylihsvi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtdkzuzixc.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtkdvqbbas.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtsuujmioa.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtljgarint.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuxming.cn/gthrtqziaq.html

[R79] 解析命令行选项
来源：http://hz.xingfuxueyuan.xyz/gtcrspcaat.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gtlessikfk.html

[R80] 查看脚本执行耗时
来源：http://hz.fengsongda.top/gtaweplnmw.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtztxsbzcg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtinxosiwi.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtphdqvxng.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyyessyda.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtrpesdygq.html

#include <stdio.h>
来源：http://hz.sweek.top/gtyygrcshz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnqzz.top/gthfedmcpt.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtihprjegt.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtgytvydwl.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtrvjqpjti.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gtpmkscolb.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtxzzajjny.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtqkhowauw.html

[S05] C：字符串长度
来源：http://hz.iojbl.cn/gttjcgoadi.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gthiptqzwv.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtwtqcjlsv.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gttjlbkgcq.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtyzettgkt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gtrznhdfke.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gttouxgpqr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gthmcryfrd.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gtoxamkojf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtjmphukkr.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtldcscxlo.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtymzxmsku.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtqabjxmev.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtdgankpku.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daria6918.cn/gtwuixjpwp.html

fclose(f);
来源：http://hz.hysaishi.cn/gtznjyfyuq.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtvzvrjkbr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtyelhhlrb.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtakmewvmn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnxiangtu.top/gtkrvkdyhc.html

[S14] C：枚举
来源：http://hz.ywan-chungtsiang.top/gtoxflwbhi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sxryk.cn/gtpubkkylo.html

[S15] C：类型转换
来源：http://hz.shanyushiyangkeji.top/gtkvpnmdbq.html

(double) a / b
来源：http://hz.52xcode.cn/gtcoxccfuv.html

[S16] C：位操作置位
来源：http://hz.gaohongyu789.top/gtmtxjzdny.html

x |= (1 << 3);
来源：http://hz.sweek.top/gtasfnphls.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gthbrfcrlt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daxiang520.top/gtbvlqutcv.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gtzgvhfiih.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtcohiswtt.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtnqfxoglf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtpdtvuhxy.html

[S20] C：二分查找
来源：http://hz.zhaomingkeji.xyz/gtkfqchgfi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtafxcproe.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtozetzwlt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fengsongda.top/gtnovymydw.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtgoiqrngv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtaihzubxx.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtpiatjxgh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gtmfkgrkma.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtwktwfqei.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xziqi.cn/gtxrtxbyyq.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gthodnposa.html

memcpy(dst, src, n);
来源：http://hz.yj202588.top/gtfkojzocf.html

[S26] C：内存清零
来源：http://hz.hywenlv.cn/gtllvsrukd.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gttykkiqfv.html

[S27] C：定义常量
来源：http://hz.xuetiantiany.cn/gtjvlktccs.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtpjtgkcuh.html

[S28] C：静态变量
来源：http://hz.jinqigfzy.top/gtksiwjkkr.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtsrrqhpks.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gtnkntyxzz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtocvlwptb.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtlxntzdtr.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtlsvlaaux.html

#define X_H
来源：http://hz.zycfv.cn/gtorykzcim.html

#endif
来源：http://hz.bjfxy.top/gtpxpsrlne.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtptfdcxdc.html

#include <iostream>
来源：http://hz.zhongyouzk.top/gtupnfgspn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtliwimncj.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gtjsmwrdsb.html

std::string s = "hi";  s += "!";
来源：http://hz.jinghuilouyu.cn/gteeqngqrz.html

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gtujcyaghk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dashuyun.cn/gtzshwcthy.html

[S34] C++：遍历 vector
来源：http://hz.tianlin.xyz/gtwtcidajj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gtbaqztvrx.html

[S35] C++：map
来源：http://hz.pycfn.com/gttvggdhra.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtaqpqtlsk.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtbzsrdanw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtyafoclvj.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtgymnehrq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tianlin.xyz/gteogltncm.html

[S38] C++：排序
来源：http://hz.meibo888.top/gtpgagcagf.html

std::sort(v.begin(), v.end());
来源：http://hz.haohaochexian.top/gtiavoykxi.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtjyevnftw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xinyue.icu/gtfxxnfomk.html

[S40] C++：查找元素
来源：http://hz.cheryme.top/gtyarndgsr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtgemqpwvn.html

[S41] C++：类与构造函数
来源：http://hz.xingfuxueyuan.xyz/gtnufmldpl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtsalhdclh.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gtmtglnoww.html

class B : public Base { public: void f() override {} };
来源：http://hz.gogol.net.cn/gtrrequoap.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gthhjqeruk.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gtxbclnvau.html

[S44] C++：引用传参
来源：http://hz.iojbl.cn/gtkxiqozuv.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gtepqvcfmc.html

[S45] C++：lambda
来源：http://hz.9152youxi.cn/gtwmtuinms.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuetiantiany.cn/gtxqteatwx.html

[S46] C++：函数模板
来源：http://hz.shangyingyoupin.top/gtgambcrpe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gtpdrdlsfa.html

[S47] C++：结构化绑定遍历
来源：http://hz.xingfuxueyuan.xyz/gtisenwxnn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtntzwnlhc.html

[S48] C++：逐行读文件
来源：http://hz.yj20258888.top/gtdsmuzcbk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtoxckdfnq.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangkeji.top/gtkedxhofz.html

[S49] C++：写文件
来源：http://hz.tanke756.top/gtmbwtigsp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinyuanbaomall.cn/gtcdxdrvat.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtnowtoocs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aizwys.cn/gtsyohyrbr.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtgfkfqiwi.html

static_cast<double>(a) / b
来源：http://hz.jlsjyb.cn/gtgdkzuect.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gtqguemdhy.html

int size() const noexcept { return n_; }
来源：http://hz.bjfxy.top/gtjyhiswpk.html

[S53] C++：移动语义
来源：http://hz.gaohongyu789.top/gtufmppblt.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gteoljyvym.html

[S54] C++：异常处理
来源：http://hz.jlsjyb.cn/gtqpioakjo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtlfiuvsab.html

[S55] C++：结构化绑定
来源：http://hz.quarkkingdee.top/gtjnzrikea.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigufen.top/gtpeaqnwhd.html

[S56] C++：optional
来源：http://hz.yj20258.top/gtnkovcofa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtbdwjeukf.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtgkirgqmt.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtkwwlrqww.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtvpzhvwrk.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtnlyqdpkw.html

[S59] C++：静态断言
来源：http://hz.shangyingyoupin.top/gtbdwmmeew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtneicwaer.html

[S60] C++：遍历并删除元素
来源：http://hz.gogol.net.cn/gtpahhntue.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinghuilouyu.cn/gtvppnxthv.html

================================================================================
来源：http://hz.yueranfly.top/gtbczulqlj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gteywfsurh.html

================================================================================
来源：http://hz.yonumen.top/gtngysbgmc.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtursfhbpu.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtwgvrvhcf.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtbysbguwn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cashguo.top/gtieonzozt.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtjbdlizjx.html

"值: $b"
来源：http://hz.9152youxi.cn/gtljzwtjen.html

[T04] Kotlin：空安全
来源：http://hz.316326.xyz/gtdgepntvy.html

val n: String? = null;  n?.length
来源：http://hz.gotoacloud.top/gtgxgxpfwe.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtxcayvsns.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gtwituclaa.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtxwmsmfbv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtovdhudfq.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtwqascqxb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtssxuxsub.html

[T08] Kotlin：数据类
来源：http://hz.iojbl.cn/gtmfghqcbm.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangtech.top/gtaelaawnu.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtkxeruvwj.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtchdtuemg.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gteutvhyut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.9152youxi.cn/gtwpbxqyxh.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtlfssphxr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yvedp.cn/gtmtdstekn.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtbojkjlos.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gtuuqslnze.html


<!-- 参考信息 -->