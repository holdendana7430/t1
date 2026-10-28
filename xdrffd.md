代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daria6918.cn/gtatqtbgwe.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtkzmoxcep.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhaomingkeji.xyz/gtuykgiuli.html

[R09] 字符串比较
来源：http://hz.smart0.xyz/gtalgsmyyz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gthlknwfpx.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtfkqiauao.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.havefunace.top/gtsncotkbh.html

[R11] case 多分支
来源：http://hz.shzxlz.cn/gtnxcrcoqc.html

case "$1" in
来源：http://hz.yanxiufei.cn/gtrzcagvgy.html

start) echo "启动" ;;
来源：http://hz.jyoumei.cn/gthscnktau.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gtahhbegrp.html

*)     echo "未知命令" ;;
来源：http://hz.xingfuxueyuan.xyz/gtuqffdczk.html

esac
来源：http://hz.yanxiufei.cn/gtfpvklqfn.html

[R12] for 遍历文件
来源：http://hz.svipenyu.cn/gtrkeyndcp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gtkbkzxupr.html

[R13] for 计数循环
来源：http://hz.dianchejie.cn/gtphyscguy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtrtnssxlf.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtuxoqmcch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtebcaggbp.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtarwztsqi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtnaelnxhu.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtahepwqml.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yonumen.top/gtbqzumkks.html

[R17] 数组定义与取值
来源：http://hz.zhijiandao.cn/gtddhuddny.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gttavmqyex.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtpsbxkeod.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydzc1.top/gtstmrvtvu.html

[R19] 数组长度
来源：http://hz.vqdsnc.cn/gtsmhrhenl.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtdranfpty.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangkeji.top/gtpjfusudx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtejpyytlj.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtfucclork.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtsyrnsogl.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtjlqvgpch.html

echo "${s:0:5}"
来源：http://hz.havefunace.top/gtzbjopock.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtamcdrfhy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aizwys.cn/gtawjsoqyb.html

[R24] 大小写转换
来源：http://hz.aibaodan.cn/gtgeebbzgn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hysaishi.cn/gtnwfutjwj.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhiwuduotai.top/gtzejchwdw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aizwys.cn/gtgggguyel.html

[R26] 命令替换
来源：http://hz.jqgufenzy.top/gtuwqlzcqm.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gthsbnkzfw.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtkpokgqlp.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtzpwpsrnm.html

[R28] 浮点运算
来源：http://hz.havefunace.top/gtqbnxrqql.html

echo "scale=2; 10/3" | bc
来源：http://hz.yvedp.cn/gtibafxvux.html

[R29] 定义函数
来源：http://hz.chenjidiqi.icu/gtweueynwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtlknykaah.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtqhiejgja.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gtnkipkkov.html

[R31] 局部变量
来源：http://hz.havefunace.top/gtikqpqbza.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gtcfxzgrpc.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtjrltzccp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtwmvwsxct.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtlzcqpnhq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtamnlxvtm.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gthvzjknqj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtzvzvycxw.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtjyvoypcw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnxiangtu.top/gtugbwqmkc.html

[R36] 并发执行多个任务
来源：http://hz.9152youxi.cn/gtpykglxcm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gotoacloud.top/gtmpsebbjw.html

[R37] 把输出赋给变量
来源：http://hz.aibaodan.cn/gtvvbvkxas.html

files=$(ls -1)
来源：http://hz.pycfn.com/gtywrlgfbi.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtfllwglwo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtyylloicj.html

[R39] 重定向标准输出与错误
来源：http://hz.svipenyu.cn/gtrnvpyctg.html

cmd > out.log 2>&1
来源：http://hz.tanke756.top/gtihegkqfu.html

[R40] 追加写日志
来源：http://hz.zhongyouzk.top/gtvzkmaxxu.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtwzzzfsmt.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtqpgpjllb.html

cmd >/dev/null 2>&1
来源：http://hz.zycfv.cn/gtaerhipsh.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtetwgaqqq.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtsgzpxbtm.html

[R43] 按名字查找文件
来源：http://hz.cheryme.top/gtelrzgwhr.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gttsvyuxrh.html

[R44] 按修改时间查找
来源：http://hz.xziqi.cn/gtbnsvzeak.html

find . -mtime -7 -type f
来源：http://hz.jlsjyb.cn/gtjhzehrgi.html

[R45] 批量删除
来源：http://hz.hnqzz.top/gtuvacosuc.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gtnlmunbpv.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtxbhiuctx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenzaomai.com/gtyoieunub.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtrlpijrda.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aizwys.cn/gtfkastpxv.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gtuosrjsgh.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtfiejwrfg.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gthtpkjtwb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.redwolf501.top/gtqvsmkfro.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gtmjezazhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nanxinkj.top/gtxpaptxns.html

[R51] 排序去重取前几
来源：http://hz.pycfn.com/gtswipmxnz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtobyzctva.html

[R52] 统计行数
来源：http://hz.pycfn.com/gtcjrwtwcp.html

wc -l a.txt
来源：http://hz.cashguo.top/gtmfctpwaz.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtqsyctsff.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sysykeji.top/gtapfuzych.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtbicsffrs.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtofodoxrn.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtocjxfocw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hongshengwenyu.top/gterpwllzu.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtjmylcosa.html

scp file user@host:/path/
来源：http://hz.hysaishi.cn/gtramgwnzb.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtbqtjgmrm.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtuncnytow.html

[R58] 下载文件
来源：http://hz.yj20258.top/gtxhgjtrfm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtkxbhabxz.html

[R59] 发 POST JSON
来源：http://hz.sxryk.cn/gtmseeghav.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtpkplmybb.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtfaaqboto.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtlewysqeu.html

[R61] 磁盘占用
来源：http://hz.sweek.top/gtqpzzebtu.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtfxktuakn.html

[R62] 找最占空间的文件
来源：http://hz.snrcjt.cn/gtfiofngoi.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtfxfnnqbm.html

[R63] 内存与进程
来源：http://hz.zhongyouzk.top/gtcyiflsic.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gtrobfaqwx.html

[R64] 结束进程
来源：http://hz.yvedp.cn/gtlwhkrxyb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yanxiufei.cn/gtjpztwnll.html

[R65] 查看端口占用
来源：http://hz.sxryk.cn/gthfawfmrh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtybzrvlvw.html

[R66] 定时任务
来源：http://hz.tianlin.xyz/gtrzdcqzxy.html

crontab -e;  crontab -l
来源：http://hz.yonumen.top/gtjbcffvci.html

[R67] 生成随机十六进制串
来源：http://hz.zhixingplan.top/gtkasekieq.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gticqjdbdw.html

[R68] 计算文件校验值
来源：http://hz.cucudq.cn/gtkndyevtn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtnjzufimn.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtiwfxrlgw.html

head -c 16 /dev/urandom | base64
来源：http://hz.dianchejie.cn/gtfxfbbznp.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtxkndhxba.html

date +%s;  date -d @1700000000
来源：http://hz.52xcode.cn/gtcpdcvkjw.html

[R71] 日期格式化
来源：http://hz.yj202588.top/gtelguycen.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cheryme.top/gtkgztovvl.html

[R72] 等待端口就绪
来源：http://hz.zhijiandao.cn/gtmgrmdues.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtvnwztusi.html

[R73] 分割大日志
来源：http://hz.ybcxt.top/gtbafqsiol.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gthduznclc.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gttafzuwor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenzaomai.com/gtdrjziaka.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtqdumgdns.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtekkszdds.html

[R76] 使用临时文件
来源：http://hz.guannengcc.top/gtzevefjbf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtwsesnsij.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtdxajlqom.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtrezkvise.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtpoifudnb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtkbwfsfgc.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtftqdejsp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gtldvrxtha.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtxbkidkru.html

time ./run.sh
来源：http://hz.hnxiangtu.top/gthitfiznm.html

================================================================================
来源：http://hz.chenzaomai.com/gttenxkssr.html

S. C / C++ 专题
来源：http://hz.zhoulong.xyz/gtjzwxubuv.html

================================================================================
来源：http://hz.wangdashe.top/gtiwjynign.html

[S01] C：Hello World
来源：http://hz.zhixingplan.top/gtlveqlbkh.html

#include <stdio.h>
来源：http://hz.ybcxt.top/gtnvqaezil.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guannengcc.top/gtzsitgilk.html

[S02] C：变量与格式化输出
来源：http://hz.zdqjudy.top/gtigamojcc.html

int a = 10; printf("%d\n", a);
来源：http://hz.jiagoushi.top/gtatfjkljo.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gttdjvbvel.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtfudqwqhx.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtwkbhlruw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangshuangyany.cn/gtmshsxnah.html

[S05] C：字符串长度
来源：http://hz.haohaochexian.top/gtbizerovw.html

strlen(s)
来源：http://hz.yj20258888.top/gtebmjawqw.html

[S06] C：字符串比较
来源：http://hz.jianghu66.top/gtmsulznii.html

strcmp(a, b) == 0
来源：http://hz.chenzaomai.com/gtojnewfyb.html

[S07] C：数组遍历求和
来源：http://hz.jqgfzy.top/gtfnnnhkbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gtiyurwgmb.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtcnwhmykh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtkftemils.html

[S09] C：结构体定义与初始化
来源：http://hz.shzxlz.cn/gtmtlvocsl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.vqdsnc.cn/gtvmumebtn.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtzvfxiikw.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtfsfgbbtc.html

[S11] C：逐行读文件
来源：http://hz.shzxlz.cn/gtlnuszsak.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtjpglspbt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ybcxt.top/gtnjtwcawx.html

fclose(f);
来源：http://hz.fengsongda.top/gtixvjbiop.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtbddgqjuw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gthqewzmhm.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtretyrpec.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtxzaukrds.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gtnpvpaeow.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.redwolf501.top/gtfhmsybah.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtuukvvecp.html

(double) a / b
来源：http://hz.zycfv.cn/gtspkoklym.html

[S16] C：位操作置位
来源：http://hz.cashguo.top/gtvkfaaadi.html

x |= (1 << 3);
来源：http://hz.jqgfzy.top/gtkwvvtpwt.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtzbhkmytq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtuqeyqjfh.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gthswsgqjg.html

int main(int argc, char **argv)
来源：http://hz.aizwys.cn/gtjxuoyess.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtvivlvltq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtybgwahpy.html

[S20] C：二分查找
来源：http://hz.yuxming.cn/gtwmynqdgv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtqejikavt.html

[S21] C：字符类别判断
来源：http://hz.shangyingyoupin.top/gtlzemorgb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xylfe.cn/gthbxndbba.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtbawhtscl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtfhuzsild.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gteroobyvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtqxysdfjj.html

[S24] C：获取本地时间
来源：http://hz.yj202588.top/gtcwqcgbzx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.meibo888.top/gtygyftcke.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtlgakkcbc.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gtfrfnnzeu.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gthaceshma.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtkllqbnkd.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtgvwobwtc.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtakpmjhty.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gtmsiduqwi.html

static int counter = 0;
来源：http://hz.nwbrower.top/gtyirmheni.html

[S29] C：变参函数
来源：http://hz.guannengcc.top/gtekiacuda.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cheryme.top/gtbblwelhr.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtqtynhvvo.html

#ifndef X_H
来源：http://hz.shuidangran.top/gthbfmnllm.html

#define X_H
来源：http://hz.guowangkeji.top/gtnfawutpv.html

#endif
来源：http://hz.pycfn.com/gtgwpzahbc.html

[S31] C++：Hello World
来源：http://hz.hammf.cn/gtmulmrnpy.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtxkonulbp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.0kj1m.cn/gteaoayehg.html

[S32] C++：字符串
来源：http://hz.tian-w.cn/gtgrqvricb.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtlnujjams.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtyntpzlcp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhiwuduotai.top/gtvjniyytj.html

[S34] C++：遍历 vector
来源：http://hz.yvedp.cn/gtlxadvjed.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtzfatixgq.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtlbgrdcic.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtjwlfdtjh.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtknztcpjv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtjoprpnme.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gtdpzhynzw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gthydaybbc.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtdhpattec.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtlabeylqo.html

[S39] C++：自定义比较器排序
来源：http://hz.yonumen.top/gtvopghfhi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yongpay.top/gtcckosrcc.html

[S40] C++：查找元素
来源：http://hz.haohaochexian.top/gtsnxnrbcr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shuidangran.top/gtbrfrfbhk.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtjnlujucn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigfzy.top/gtwegmqxrc.html

[S42] C++：继承与虚函数
来源：http://hz.cucudq.cn/gtjhrsuawq.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtsodsawyp.html

[S43] C++：智能指针
来源：http://hz.nanxuanxn.top/gtahscgvin.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gttpwmtkze.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gtvsrhtjpc.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtoecsautu.html

[S45] C++：lambda
来源：http://hz.birdmap.top/gtjjtimlpu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gttypxfpsf.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtxzessqgv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gogol.net.cn/gtcrbzmmdn.html

[S47] C++：结构化绑定遍历
来源：http://hz.xingfuxueyuan.xyz/gttlkbpviu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtvubmnscu.html

[S48] C++：逐行读文件
来源：http://hz.jianghu66.top/gtuaazwkqb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtjkzphqoh.html

while (std::getline(in, line)) { }
来源：http://hz.yvedp.cn/gtjbehahgp.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtgqvjqqfn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.316326.xyz/gtipdrakdy.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtjrwhxemv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhiwuduotai.top/gtbhuejcyc.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtaonzqsqf.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gtbgdzseuz.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtvmfbaysd.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtlxonuduo.html

[S53] C++：移动语义
来源：http://hz.pengpengdd.cyou/gtsxjiepju.html

std::vector<int> w = std::move(v);
来源：http://hz.jinyuanbaomall.cn/gtpsypvhis.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtelbtoqfn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgufenzy.top/gtxxjbwuxj.html

[S55] C++：结构化绑定
来源：http://hz.nanxinkj.top/gtvrmfqxcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.bjfxy.top/gtmnsskkcd.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gttepxjrbo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuetiantiany.cn/gthxcmhdvo.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gtvwumtxmw.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtkrajtodm.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtjvxbgjhq.html

namespace ns { int f() { return 1; } }
来源：http://hz.tanke756.top/gtnavclwad.html

[S59] C++：静态断言
来源：http://hz.hywenlv.cn/gtssaltbfg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigfzy.top/gtwokrnhdx.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtfwrlrtls.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtygtcpeog.html

================================================================================
来源：http://hz.ydzc1.top/gtnwalbqid.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.smart0.xyz/gtpwmdlrol.html

================================================================================
来源：http://hz.pycfn.com/gtkxcmxsqz.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtsshfangq.html

println("Hello")
来源：http://hz.zycfv.cn/gtcqhkhmzk.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtruztbotl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gtelntwiey.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtbellvwoz.html

"值: $b"
来源：http://hz.tian-w.cn/gtzfwlonzz.html

[T04] Kotlin：空安全
来源：http://hz.jqgfzy.top/gtzuokqxlt.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtmkcxzpxp.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtgiiudbac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258.top/gtkxzzikwh.html

[T06] Kotlin：集合映射
来源：http://hz.pengpengdd.cyou/gtlfuidqnz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cdnleiting.top/gtzyogwdyg.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigfzy.top/gtjovxubll.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinghuilouyu.cn/gtyrbxennv.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gtuxbdwprc.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtiycnemfp.html


<!-- 参考信息 -->