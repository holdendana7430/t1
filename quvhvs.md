代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtmhxcqhxe.html

[Q73] 查看表状态
来源：http://hz.ybcxt.top/gtiqixkilg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxinkj.top/gttkbctczm.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtjhhymflx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sysykeji.top/gtnnufawmd.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gttklygzzd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtgpigfjwt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtdbqglpfy.html

[Q76] 按天统计
来源：http://hz.svipenyu.cn/gtoxhytueh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jianghu66.top/gttzeffocg.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtfhaiejnt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258888.top/gtdktgzrmy.html

[Q78] 当前时间
来源：http://hz.gzhubu.top/gtekymdmxb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jianghu66.top/gtnomqunvg.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtszqiubcy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gtyxxfutac.html

[Q80] 字符串截取
来源：http://hz.aibaodan.cn/gtcdsxjsbw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtsrczuqap.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtaslwpgeu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yangfankeji.com/gtczkoodfe.html

[Q82] 字符长度与字节长度
来源：http://hz.xuetiantiany.cn/gtheeqkedf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenzaomai.com/gttqwnkmeu.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtljeuqnak.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gthnlbnxty.html

[Q84] 去除首尾空格
来源：http://hz.zhoulong.xyz/gtqckrzqow.html

SELECT TRIM(name) FROM users;
来源：http://hz.redwolf501.top/gtdyubrovb.html

[Q85] 数值取整
来源：http://hz.jianghu66.top/gtluftutge.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnxiangtu.top/gtrhgcxiek.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtwdvrwise.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtxkuhcaej.html

[Q87] JSON 字段做条件
来源：http://hz.cdnleiting.top/gtgynduviq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtkifaidzu.html

[Q88] 行转列（条件聚合）
来源：http://hz.jlsjyb.cn/gteafsunqm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gticucczsv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.svipenyu.cn/gtmkksbnzn.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtbkxkdeng.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.316326.xyz/gtaglqhpyg.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtdkdotwaa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.quarkkingdee.top/gtbcbbninz.html

================================================================================
来源：http://hz.yvedp.cn/gtjavzkiom.html

R. Bash 专题
来源：http://hz.dianchejie.cn/gtdorbkjko.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwcwpfjec.html

[R01] shebang 与严格模式
来源：http://hz.9152youxi.cn/gtedelineq.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gtibdtnkws.html

set -euo pipefail
来源：http://hz.wangshuangyany.cn/gtahzrtefj.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtxmnrlsjc.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtnbgsjbym.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtifqijfuy.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtdzhqdrgy.html

[R04] 位置参数
来源：http://hz.yongpay.top/gtdvjusodm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtwjcdryiv.html

[R05] 参数默认值
来源：http://hz.0kj1m.cn/gtlbkdfchq.html

name="${1:-default}"
来源：http://hz.ivvv.top/gtgwtklysx.html

[R06] 判断命令是否存在
来源：http://hz.cqqwz.cn/gtevxfnkvl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtuvvqawjt.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtgqqnkrve.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtidtrcesx.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gtpusyvrmq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtzmjvwucf.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gtazmfkqnl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtyrrbyxro.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtmuotmxka.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtatabltmy.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtjxcuhsjd.html

case "$1" in
来源：http://hz.hywenlv.cn/gtlewufzac.html

start) echo "启动" ;;
来源：http://hz.wangshuangyany.cn/gtreyihdpc.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtttdhnnam.html

*)     echo "未知命令" ;;
来源：http://hz.shzxlz.cn/gtyvpzhryg.html

esac
来源：http://hz.ivvv.top/gtoppktxjw.html

[R12] for 遍历文件
来源：http://hz.xingfuxueyuan.xyz/gtqlrgxzlm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gtdltwuwyi.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtbkmrkigv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aizwys.cn/gthnzldbog.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtetrcwstp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtflspnvvq.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtphubaspr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtjvspawxl.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtqthsnqeg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258.top/gtsudcorns.html

[R17] 数组定义与取值
来源：http://hz.xylfe.cn/gtxyepjfii.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gtkxnwdoac.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtkgnopocx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ppjwa.cn/gtakjseuny.html

[R19] 数组长度
来源：http://hz.smart0.xyz/gtqpaklkxw.html

echo "${#arr[@]}"
来源：http://hz.ehwqpu.com/gtpsvreick.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gtmjtkdxkb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenzaomai.com/gtmvjaovbn.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtdvewhqgn.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtlnghkjam.html

[R22] 截取子串
来源：http://hz.gzhubu.top/gtfodfsyaz.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtcewrdldx.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gtlfpuqkrk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtujhamhrq.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gtnrcaqnge.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnxiangtu.top/gtyuzemuvw.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtteyzeybd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtclyjoyrf.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtdnnjvwmb.html

now=$(date +%F); echo "$now"
来源：http://hz.aizwys.cn/gtdulpdzdh.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtvgowqvvq.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtjmlggxig.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtmzwgtqrp.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtpubmdvex.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtqadqmmrv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtqjqaohhf.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtdiafrnkh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gtszaueolk.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtgxsbernw.html

f() { local x=1; echo "$x"; }
来源：http://hz.ehwqpu.com/gtalvijpkq.html

[R32] 参数个数校验
来源：http://hz.iojbl.cn/gtkmeejtkv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtszwybxwe.html

[R33] 捕获错误并提示行号
来源：http://hz.quarkkingdee.top/gtrsmracdn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtzrslgzlx.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtwzxrvxwv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gthxrqqkje.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtidprgwwe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtyqodgtol.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtfoauuelv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtczdjjycf.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtapvobxxy.html

files=$(ls -1)
来源：http://hz.wangdashe.top/gtbtodxgul.html

[R38] 管道串联
来源：http://hz.zhengqikj.top/gtnjksonwr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtyotlgerv.html

[R39] 重定向标准输出与错误
来源：http://hz.hongshengwenyu.top/gtdkibwhpk.html

cmd > out.log 2>&1
来源：http://hz.hnqzz.top/gtokirewhx.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtxsuhswhb.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtxbfpbtsc.html

[R41] 丢弃输出
来源：http://hz.tian-w.cn/gttszdkejl.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gtgxnaytcd.html

[R42] 输入重定向
来源：http://hz.zhijiandao.cn/gttqzpynnr.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtsrfyrnqr.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtmofrdonb.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtazjalike.html

[R44] 按修改时间查找
来源：http://hz.xingfuxueyuan.xyz/gtmhvgmpsb.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gttpttmstl.html

[R45] 批量删除
来源：http://hz.dianchejie.cn/gtkyxriiin.html

find . -name "*.tmp" -delete
来源：http://hz.xylfe.cn/gtalyjyuyt.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtrppdzldd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtszhphtpj.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtzqhpcxot.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtvriaalzg.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtsxvirxwa.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtgutnvxgy.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtmvyiakmk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aibaodan.cn/gtxmfunybd.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtflogijie.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yanxiufei.cn/gtikuiqprj.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtipvazioi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gtzmqizgqd.html

[R52] 统计行数
来源：http://hz.sysykeji.top/gthvadzjlr.html

wc -l a.txt
来源：http://hz.yongpay.top/gtkpzxeobj.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtyiszsgpy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.feifeiyinyue.top/gtqjwnehfa.html

[R54] 比较两个文件
来源：http://hz.fengsongda.top/gtlkzodmjw.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtfxrtdehh.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gtcmlenduc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fengsongda.top/gtikhgelqr.html

[R56] 远程拷贝
来源：http://hz.ppjwa.cn/gtgkxxgkax.html

scp file user@host:/path/
来源：http://hz.tianlin.xyz/gtqowaqesh.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtcaxlqacp.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtioqlvyml.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtdipxzhfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jiagoushi.top/gtjubvmftu.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gtcxaooyii.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hysaishi.cn/gtugckquly.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtluyznoqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangkeji.top/gtcaispvkn.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gtvktbnuvt.html

df -h;  du -sh *
来源：http://hz.xuetiantiany.cn/gtdiywohbn.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtuckcmwbz.html

du -ah . | sort -rh | head -10
来源：http://hz.pycfn.com/gtlnzxggwx.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gtsadbxkeb.html

free -h;  ps aux | grep nginx
来源：http://hz.dianchejie.cn/gtqsttsawl.html

[R64] 结束进程
来源：http://hz.jqgufenzy.top/gtuxklemnc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dashuyun.cn/gtlxrrpiug.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtuexsrfiu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtrrkkwpap.html

[R66] 定时任务
来源：http://hz.daria6918.cn/gtqhprmcll.html

crontab -e;  crontab -l
来源：http://hz.hnqzz.top/gtsxaiquod.html

[R67] 生成随机十六进制串
来源：http://hz.feifeiyinyue.top/gtsoswuvyb.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtjtifltcu.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtehvdtize.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtatwekquy.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtsejyvlqc.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtlxqpdkgt.html

[R70] 时间戳与互转
来源：http://hz.hnqzz.top/gtcksbiqfl.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gtfawmfhso.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtictmrzjt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtvcdiyful.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtmnwdwign.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtsjzbsjyz.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gtfrzwpfpx.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtwstasfuv.html

[R74] 批量重命名
来源：http://hz.gaohongyu789.top/gtqmfapqhp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhoulong.xyz/gtibbdmefs.html

[R75] 导出环境变量
来源：http://hz.yanxiufei.cn/gthryfzggw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtbsgvdhcz.html

[R76] 使用临时文件
来源：http://hz.svipenyu.cn/gtolerdbou.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gttoaxjniz.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtfahdhadn.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtebvfwrpi.html

[R78] 交互式菜单
来源：http://hz.ivvv.top/gtzcboqtnd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtqweuqxtv.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtuzlwrkhz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shuidangran.top/gtqalpbire.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtkqarfqmt.html

time ./run.sh
来源：http://hz.cheryme.top/gtwkxhfoph.html

================================================================================
来源：http://hz.jiagoushi.top/gtiiygynch.html

S. C / C++ 专题
来源：http://hz.yj20258888.top/gtpmqipstd.html

================================================================================
来源：http://hz.zycfv.cn/gtcqxqugcm.html

[S01] C：Hello World
来源：http://hz.meibo888.top/gtrjlbloxg.html

#include <stdio.h>
来源：http://hz.guowangkeji.top/gtlrgvterb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jyoumei.cn/gtboofhxxz.html

[S02] C：变量与格式化输出
来源：http://hz.sufxvd.cn/gtpzhdlinh.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtxtpkcgyl.html

[S03] C：读入整数
来源：http://hz.ybcxt.top/gthycloiku.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtaylbyebp.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gteuavceak.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuetiantiany.cn/gtwtfpyawq.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtuvvbjllk.html

strlen(s)
来源：http://hz.tian-w.cn/gtrwyzmsvw.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gthqaodtni.html

strcmp(a, b) == 0
来源：http://hz.yanxiufei.cn/gtxggwtoae.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtaqbmzvnb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtglmarxhm.html

[S08] C：动态内存分配与释放
来源：http://hz.yanxiufei.cn/gtfvbaemww.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtvinddzhe.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gtwyqivcra.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtwjwlcnbu.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtsypkjbju.html

int *p = &a;  *p = 5;
来源：http://hz.jqgfzy.top/gtchzebiyn.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gtgsqckakp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtyrkbnkch.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shangyingyoupin.top/gtkoxtjiat.html

fclose(f);
来源：http://hz.dianchejie.cn/gtgaqlunvg.html

[S12] C：写文件
来源：http://hz.kuanghao11.cn/gtkhnvjrfy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.svipenyu.cn/gtbkhkuklc.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtpwlwxyli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fzhhl.top/gtajleryjb.html

[S14] C：枚举
来源：http://hz.gaohongyu789.top/gtffqmzjry.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtgrqyvzcx.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtfcbxgdfh.html

(double) a / b
来源：http://hz.fzhhl.top/gtrmcezobj.html

[S16] C：位操作置位
来源：http://hz.jlsjyb.cn/gtdqobjmrn.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtwsizcecb.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtxjuyllmw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sysykeji.top/gtexlmpafv.html

[S18] C：命令行参数
来源：http://hz.ppjwa.cn/gtmwahkwcz.html

int main(int argc, char **argv)
来源：http://hz.ydzc1.top/gtslmorxrp.html

[S19] C：快速排序
来源：http://hz.shzxlz.cn/gtlllnynpg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtamdazrat.html

[S20] C：二分查找
来源：http://hz.ydzc1.top/gtmxmnpyot.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtyulgbxoa.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangtech.top/gtvtgcnjnu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtkyseuvxm.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtbxnnsosr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gtcxwkxujb.html

[S23] C：随机数
来源：http://hz.xziqi.cn/gtjfzedrbd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.9152youxi.cn/gtzjoumjgx.html

[S24] C：获取本地时间
来源：http://hz.ivvv.top/gtwnkwvqir.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuanzx.com/gtrkpwarwq.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtpltnwswk.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtkfcjgmui.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gtfzkdhbbh.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtwhooqmpk.html

[S27] C：定义常量
来源：http://hz.hfpthk.cn/gtfmjucnps.html

const double PI = 3.14159;
来源：http://hz.nwbrower.top/gtfxsubore.html

[S28] C：静态变量
来源：http://hz.nanxinkj.top/gtpgddbnxp.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtduoervfd.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtrvaavvfq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtqonzzido.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtbkvyjdva.html

#ifndef X_H
来源：http://hz.hongshengwenyu.top/gteklmigfg.html

#define X_H
来源：http://hz.cdnleiting.top/gtgjqjskds.html

#endif
来源：http://hz.feifeiyinyue.top/gthauneymm.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtpquhxnls.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtrwuzlogp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtltpcvxcu.html

[S32] C++：字符串
来源：http://hz.hysaishi.cn/gtpqovkaqp.html

std::string s = "hi";  s += "!";
来源：http://hz.ydjk.org.cn/gtnnqhexcv.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtmczgqztu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtsreiufua.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtmnxojfzq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtjjmkllpf.html

[S35] C++：map
来源：http://hz.hammf.cn/gtcwnmymhc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtoregbxfk.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtlcznuczb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtktoapijk.html

[S37] C++：set
来源：http://hz.birdmap.top/gteeczwqoo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtbdugfjmx.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtgulaeipn.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtmavoynjs.html

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gttatjoraj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtqemhgeik.html

[S40] C++：查找元素
来源：http://hz.jinyuanbaomall.cn/gtjffwezbw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gttetzgple.html

[S41] C++：类与构造函数
来源：http://hz.cheryme.top/gtfsfqxvwg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtozslllvz.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gthjudbhhr.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gthrvkttql.html


<!-- 参考信息 -->