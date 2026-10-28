代发 wailian999

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtoxhxzsxj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtxkcmgrnj.html

[Q81] 字符串替换
来源：http://hz.yueranfly.top/gtevthsdhd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sxryk.cn/gtuyzeibcz.html

[Q82] 字符长度与字节长度
来源：http://hz.shzxlz.cn/gtrbqcldeg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtkrosdnfr.html

[Q83] 大小写转换
来源：http://hz.zhengqikj.top/gtrjzrqlrk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtxxcnhjvw.html

[Q84] 去除首尾空格
来源：http://hz.xylfe.cn/gtdjawmodr.html

SELECT TRIM(name) FROM users;
来源：http://hz.shzxlz.cn/gtgeroudkw.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtrhuqhepy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtkdmhhdbx.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gtqyuoickl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zycfv.cn/gtwnxavola.html

[Q87] JSON 字段做条件
来源：http://hz.fengsongda.top/gtrfyrvwxx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hongshengwenyu.top/gtcktchdfh.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtbfkegoww.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtrmqetlos.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cheryme.top/gtgiqyvfep.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtsdatcwal.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ywan-chungtsiang.top/gtlwwekiix.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtilbdogbn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zycfv.cn/gttuaswgpr.html

================================================================================
来源：http://hz.chenzaomai.com/gtadrxrqvj.html

R. Bash 专题
来源：http://hz.guannengcc.top/gtfqfsrbcl.html

================================================================================
来源：http://hz.nwbrower.top/gtkwsnayip.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtqqcgadcl.html

#!/usr/bin/env bash
来源：http://hz.pycfn.com/gtjrwvzres.html

set -euo pipefail
来源：http://hz.yj20258888.top/gtrtnqwqne.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gtfvvkgbox.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtttqwmszg.html

[R03] 只读变量
来源：http://hz.fengsongda.top/gtdwuqvnnk.html

readonly PI=3.14
来源：http://hz.tanke756.top/gtisqeovyj.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gtbpxshkqe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtzpvwyjol.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gturrafegj.html

name="${1:-default}"
来源：http://hz.hysaishi.cn/gtsbrgrdqw.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtzlahzuca.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtizmnnnxu.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtjrvvxhlj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtryqziuni.html

[R08] 数值比较
来源：http://hz.bjfxy.top/gtagjonyff.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtmtgukxtt.html

[R09] 字符串比较
来源：http://hz.zdqjudy.top/gtbgjxuhqb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtgcnmvrkc.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gtdcjeoanq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtcldkrcjp.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gtsaycclar.html

case "$1" in
来源：http://hz.jinqigufen.top/gttnwidwcq.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gtuvmpeueb.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtccqnyuaa.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtpmapmmsw.html

esac
来源：http://hz.jianghu66.top/gtiokxnohy.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtmutxdmkh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hywenlv.cn/gtjqhrdyyu.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtelbbinmn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yongpay.top/gtcaiaptbv.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gtbatyhbda.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tanke756.top/gtclpbqxwx.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtxqikfulc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtfvultpfx.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtevrsozqf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtibgmaego.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtraxxymsl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yueranfly.top/gtlezhvuth.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtvtdugdck.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtophcluog.html

[R19] 数组长度
来源：http://hz.sweek.top/gtfbwrtqbt.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtvsksgnlj.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtdqkxuvtn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtjfwtxwro.html

[R21] 字符串长度
来源：http://hz.yj202588.top/gtckkekzct.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtivxuszft.html

[R22] 截取子串
来源：http://hz.yuanzhike.top/gtkqtwvrtu.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtvrcvqosd.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gterjxomeb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhijiandao.cn/gtuntrfaxk.html

[R24] 大小写转换
来源：http://hz.sysykeji.top/gtqpsuqbeq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xinyue.icu/gtectoaepu.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtmpvmqwyp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gtmqklkzrl.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtbozjkwrr.html

now=$(date +%F); echo "$now"
来源：http://hz.tianlin.xyz/gtduxqnpjk.html

[R27] 算术展开
来源：http://hz.jinyuanbaomall.cn/gtukbeihhl.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258.top/gtmmosjoho.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtylmqamum.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigufen.top/gtdyoeplzu.html

[R29] 定义函数
来源：http://hz.zdqjudy.top/gtzvinmmla.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gtsdipcfii.html

[R30] 函数返回状态码
来源：http://hz.jiagoushi.top/gtgaatcglp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hywenlv.cn/gtmbeppcdf.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gtjicpeiep.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangshuangyany.cn/gtnflnfxrz.html

[R32] 参数个数校验
来源：http://hz.cheryme.top/gtqwtifzhy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.quarkkingdee.top/gtgjzyxokf.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtekqxepad.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtiklwrnhg.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gthjkfpccp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtgwmxlmrh.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtsbehflpb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhiwuduotai.top/gtkxzoowwz.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtqsvetguz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guowangkeji.top/gtnbwzvhhv.html

[R37] 把输出赋给变量
来源：http://hz.chenlongwang.top/gtpxdzqrff.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtfrhgtyct.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gthgognacc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hysaishi.cn/gtjxgwqvwq.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gthmpymhdx.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtozplbnap.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtatdwuukf.html

echo "log" >> out.log
来源：http://hz.jiagoushi.top/gtukxswysc.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gttgizlhnw.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtzrrxqqpi.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gtvrvjsqey.html

wc -l < a.txt
来源：http://hz.nanxinkj.top/gtdkoiuhik.html

[R43] 按名字查找文件
来源：http://hz.vqdsnc.cn/gtxqgetvsn.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gtwvzmvsra.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gtpturcnbf.html

find . -mtime -7 -type f
来源：http://hz.chenzaomai.com/gtvfuosymt.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtcvbkavmh.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gtijfgpahc.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtxgtxbvsl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtdhjobuxk.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtrqvsldgl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtxkdlrrfk.html

[R48] awk 取指定列
来源：http://hz.vqdsnc.cn/gtnnaeyzlq.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gthxkhqorg.html

[R49] awk 带条件
来源：http://hz.guowangkeji.top/gtotzdtqyv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtbyxymife.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtvulicgtn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pengpengdd.cyou/gtsfxfyqrn.html

[R51] 排序去重取前几
来源：http://hz.yangfankeji.com/gtdhvaewsj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtmoamnkzr.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gttmqyxsly.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gthkzazssk.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gtqcifpifg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daria6918.cn/gtetqefqjw.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtfudccptt.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtqtcfbjzg.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtzeefkcvd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtqworyhmu.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtgdbpaanj.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtfpmlinmg.html

[R57] 远程执行命令
来源：http://hz.316326.xyz/gtwumhsuav.html

ssh user@host 'uptime'
来源：http://hz.jyoumei.cn/gtcuphlaat.html

[R58] 下载文件
来源：http://hz.xingfuxueyuan.xyz/gtslftmyyd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtqnvsycut.html

[R59] 发 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtahswtcfe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtvmpxzykm.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtmbgnynfa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gteiuedqsq.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtzzkakvcc.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtrkvsvxbq.html

[R62] 找最占空间的文件
来源：http://hz.jlsjyb.cn/gteyzdqhjm.html

du -ah . | sort -rh | head -10
来源：http://hz.jinghuilouyu.cn/gtwpsxwltz.html

[R63] 内存与进程
来源：http://hz.ivvv.top/gtiuqdbmeb.html

free -h;  ps aux | grep nginx
来源：http://hz.quarkkingdee.top/gtvupdntpm.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtsnlpuehm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cqqwz.cn/gthzbashkc.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtgcddeppl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.havefunace.top/gtteqgdiyx.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtyhvmlpus.html

crontab -e;  crontab -l
来源：http://hz.hywenlv.cn/gtbyllfzcy.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtzzhmnhwf.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gtupnicjmh.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtewfdgdct.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gthdnivqxe.html

[R69] 生成随机密码
来源：http://hz.dashuyun.cn/gtzenotcry.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtzntjwewz.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtokzuqwms.html

date +%s;  date -d @1700000000
来源：http://hz.9152youxi.cn/gtzonbknax.html

[R71] 日期格式化
来源：http://hz.gogol.net.cn/gtbwrgtmwj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtyxczufaf.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtxyhhtusx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtdxmbbhzl.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtywmgafkc.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtixtrsxje.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtnfkwefmc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtdcarafly.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gtkkabenmi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtmhwencas.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtowfryjfx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtjifrxcxg.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtjnjpnvoo.html

read -rp "请输入: " ans
来源：http://hz.316326.xyz/gtbrqlixrx.html

[R78] 交互式菜单
来源：http://hz.shuidangran.top/gtctbuphwo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.bjfxy.top/gtxlvszpyz.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtkxqfmqfy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jlsjyb.cn/gtiraohrmp.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtpshapuss.html

time ./run.sh
来源：http://hz.chenlongwang.top/gtvjdcvbzn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnpdlllsy.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gttowuuops.html

================================================================================
来源：http://hz.daxiang520.top/gtrvoholum.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtcjetimfl.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtqqkpatpx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtydjbvvfo.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gttdtfhsne.html

int a = 10; printf("%d\n", a);
来源：http://hz.cheryme.top/gtaabslivx.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtqhkiqgjd.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtufauyuzg.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtebtbbrqu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtadflmnsd.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtkzvbvfem.html

strlen(s)
来源：http://hz.yonumen.top/gtpejjnwxa.html

[S06] C：字符串比较
来源：http://hz.zhiwuduotai.top/gtciysljkm.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtokktxkvf.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gtrruykpbt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.iojbl.cn/gtftusfpag.html

[S08] C：动态内存分配与释放
来源：http://hz.wangshuangyany.cn/gtexmfkzgg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gtsfvscqje.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtfumcrudh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtiqecbcqp.html

[S10] C：指针与解引用
来源：http://hz.jinqigufen.top/gtidgmwszf.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gtqiwuswcc.html

[S11] C：逐行读文件
来源：http://hz.jinqigufen.top/gtysfaqayv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangtech.top/gtsfhabloo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtinuklijb.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtzmtsruhk.html

[S12] C：写文件
来源：http://hz.gogol.net.cn/gtxitamdyj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhongyouzk.top/gtxefjsinq.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtvrfbiybt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gtjskbrulv.html

[S14] C：枚举
来源：http://hz.sxryk.cn/gtrbfhirvk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gtopkecuxz.html

[S15] C：类型转换
来源：http://hz.52xcode.cn/gtcnuvzuye.html

(double) a / b
来源：http://hz.bjfxy.top/gtwaioasis.html

[S16] C：位操作置位
来源：http://hz.cashguo.top/gtxmeelfwm.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtwjmphsqh.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtubkzlovj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtfkydyhiu.html

[S18] C：命令行参数
来源：http://hz.yj20258.top/gtarmkoqqt.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtkywarmiz.html

[S19] C：快速排序
来源：http://hz.fzhhl.top/gtseflajsw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtpymckcsl.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtppuhtmkm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtakkbpydu.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtvreeojjc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtfltyxfrj.html

[S22] C：字符串转数字
来源：http://hz.chenlongwang.top/gtufvvuwgi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yongpay.top/gtvrsuttds.html

[S23] C：随机数
来源：http://hz.ydjk.org.cn/gtnurltqnx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtkacysgeo.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtiibbslib.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtyrzxdkyj.html

[S25] C：内存拷贝
来源：http://hz.sufxvd.cn/gtkqfwpqeo.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtwtgikjgt.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtjunpkwiw.html

memset(a, 0, sizeof a);
来源：http://hz.ehwqpu.com/gtfwnanmpe.html

[S27] C：定义常量
来源：http://hz.yonumen.top/gtyhgamaih.html

const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gtlvvnqsvm.html

[S28] C：静态变量
来源：http://hz.c1oappe.top/gtvfigkopj.html

static int counter = 0;
来源：http://hz.zycfv.cn/gtrkcydgbz.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtpnuyidny.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtqumnqcvr.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtnergtdty.html

#ifndef X_H
来源：http://hz.xziqi.cn/gtgmzfromw.html

#define X_H
来源：http://hz.yj202588.top/gtfdyykdmn.html

#endif
来源：http://hz.hnxiangtu.top/gtacdjacwr.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtwlcdludx.html

#include <iostream>
来源：http://hz.cucudq.cn/gtebgibbui.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinyuanbaomall.cn/gtrjfytske.html

[S32] C++：字符串
来源：http://hz.hammf.cn/gttcodpfwq.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtsljgwuxh.html

[S33] C++：vector 增删
来源：http://hz.redwolf501.top/gtptpqdrgn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.quarkkingdee.top/gtlmchlcbq.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtzfnpzhxa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.meibo888.top/gtnerbsnek.html

[S35] C++：map
来源：http://hz.c1oappe.top/gteumsxlbo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtbglozlwo.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtsqofnijv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gthsdjcwyj.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtjcuyicek.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yangfankeji.com/gtwnsmeida.html

[S38] C++：排序
来源：http://hz.jiagoushi.top/gtczfacmxe.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gtialekbgu.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gtnnlprblx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sweek.top/gtqrqvcdrq.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gtltzluauj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gtwdycoxnu.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtcrdbtjdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gzhubu.top/gtykmxqkav.html

[S42] C++：继承与虚函数
来源：http://hz.hnxiangtu.top/gtboiyownb.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtzesoaodp.html

[S43] C++：智能指针
来源：http://hz.52xcode.cn/gtwxwwcadr.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtqtgkjjla.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtjajwfqhk.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gtcqomzkru.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtxvcarfpo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtuyiulnpm.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtoqlwxnud.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ppjwa.cn/gticwnyayu.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtnjsjhtww.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtehkqienk.html

[S48] C++：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtlvxovkmq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aizwys.cn/gtmqnulgwr.html

while (std::getline(in, line)) { }
来源：http://hz.andypj.xyz/gtsunwwfvf.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtmoivjgkm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtdaldblmr.html

[S50] C++：格式化数字
来源：http://hz.birdmap.top/gtkktrhkzd.html


<!-- 参考信息 -->