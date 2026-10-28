代发 wailian999

ANALYZE TABLE users;
来源：http://hz.zycfv.cn/gtgbejtrnh.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtxdahhimo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtfuztlrgy.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gtvgqjvgpq.html

SHOW INDEX FROM users;
来源：http://hz.sweek.top/gtuafxwfzs.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gteexrgony.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtoidtraue.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtggjohtwh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gthxvsyesy.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtuffgfmuz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxinkj.top/gtewodbchi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtmjpesmwu.html

[Q76] 按天统计
来源：http://hz.xziqi.cn/gtgrwcpdkn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sysykeji.top/gtoykokamv.html

[Q77] 时间加减
来源：http://hz.havefunace.top/gtgccouyxu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhijiandao.cn/gtfligivnb.html

[Q78] 当前时间
来源：http://hz.wangshuangyany.cn/gtafffruro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtpomemjup.html

[Q79] 字符串拼接
来源：http://hz.andypj.xyz/gtxienvhbh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.mhx1999.top/gtzfggibll.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtepgkhesp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtfhssiajo.html

[Q81] 字符串替换
来源：http://hz.sufxvd.cn/gtkbygolvk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fzhhl.top/gtwuebtalo.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtxntlywam.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dianchejie.cn/gtymmhtnpw.html

[Q83] 大小写转换
来源：http://hz.meibo888.top/gtdlbkgnol.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ybcxt.top/gtjxdmymrd.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gthddsojid.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuanzx.com/gtbidhvffm.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtwpvecqsz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtzfrbhkws.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtgmxxuisq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxinkj.top/gtaojuopov.html

[Q87] JSON 字段做条件
来源：http://hz.pengpengdd.cyou/gthxaazdpz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jianghu66.top/gtgucejyin.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtxhwnwqbo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gogol.net.cn/gtmwlmrrlv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtzgdtqgsh.html

[Q89] 判断表是否存在
来源：http://hz.chenjidiqi.icu/gtddtcuvde.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangdashe.top/gtuavmvkcw.html

[Q90] 生成序号列
来源：http://hz.yonumen.top/gtzshlsotk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtsbmjnjzc.html

================================================================================
来源：http://hz.52xcode.cn/gtqugoqekb.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtorjddpkp.html

================================================================================
来源：http://hz.svipenyu.cn/gtdlbkyurw.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtzncuirpa.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtlxvtwizh.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gtedwwkvvo.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtbluvouqw.html

name="Tom"; echo "$name"
来源：http://hz.fzhhl.top/gtenhwcsen.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gtkqfbhbls.html

readonly PI=3.14
来源：http://hz.redwolf501.top/gttkssvoei.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtoseabpmh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtrrlwaepy.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtpazyvynw.html

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gtuzpwtqxi.html

[R06] 判断命令是否存在
来源：http://hz.meibo888.top/gtiuoypfix.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtqbmqpkwq.html

[R07] if 判断文件
来源：http://hz.cdnleiting.top/gtootsvzyk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hammf.cn/gteytvbzzn.html

[R08] 数值比较
来源：http://hz.0kj1m.cn/gtkhsclhow.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yvedp.cn/gtfbzhjdkt.html

[R09] 字符串比较
来源：http://hz.yuanzhike.top/gtddwdpmcq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daria6918.cn/gtjneaovyz.html

[R10] 正则匹配
来源：http://hz.iojbl.cn/gtzsvoflml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yongpay.top/gtqnwuemxu.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtmxyakefe.html

case "$1" in
来源：http://hz.yangfankeji.com/gtmlcyaqac.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtkfbwsugj.html

stop)  echo "停止" ;;
来源：http://hz.quarkkingdee.top/gtehxbyalx.html

*)     echo "未知命令" ;;
来源：http://hz.birdmap.top/gtrovsfofb.html

esac
来源：http://hz.jlsjyb.cn/gtimyvoiwx.html

[R12] for 遍历文件
来源：http://hz.jianghu66.top/gtcwfbnerw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhengqikj.top/gtljhtkawq.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtckctodue.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.52xcode.cn/gtbdpqegkq.html

[R14] C 风格 for
来源：http://hz.jlsjyb.cn/gtnyfzaxeg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtufzscngx.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gtedyyuczn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.svipenyu.cn/gtwoyvxpps.html

[R16] until 等待条件
来源：http://hz.guowangkeji.top/gtvwekncam.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtkeqqexhy.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtbwcsqcht.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nanxuanxn.top/gtrjddqgmn.html

[R18] 遍历数组
来源：http://hz.hongshengwenyu.top/gtpnazolse.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnqzz.top/gtiqjkofeg.html

[R19] 数组长度
来源：http://hz.quarkkingdee.top/gthfnpzefu.html

echo "${#arr[@]}"
来源：http://hz.yj20258888.top/gtxjiumfjr.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtkflglnxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shuidangran.top/gtqrgwycqz.html

[R21] 字符串长度
来源：http://hz.tanke756.top/gtyngvrxai.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtwjwzlbll.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtuziihkyv.html

echo "${s:0:5}"
来源：http://hz.vqdsnc.cn/gtsswdfopb.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtrtqgobsi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtxzqsvpsf.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtvjjxzsfu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangkeji.top/gtecprepan.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtgqifhgdr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtulekxcbl.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtmidzedoq.html

now=$(date +%F); echo "$now"
来源：http://hz.yvedp.cn/gtkhfndumn.html

[R27] 算术展开
来源：http://hz.kuanghao11.cn/gtbzdexnlf.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtueencraw.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtsttthwon.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtbuzbcquh.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtyqbbppxt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtdmevogin.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gtverkloag.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtihdintqn.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gtpodhkloj.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtlbtpdrcf.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtxtjqpuhl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtgxpchtgk.html

[R33] 捕获错误并提示行号
来源：http://hz.snrcjt.cn/gtevzpddji.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuxming.cn/gtpxasncmd.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gthezxphoe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtthcgdmmo.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtwddmvrwy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtoyyelvto.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtwdychxaf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtkpyqxegs.html

[R37] 把输出赋给变量
来源：http://hz.daria6918.cn/gttoagkkzq.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtoxddezbj.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtyxvaqlov.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xziqi.cn/gtsdhbimrw.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtdunduait.html

cmd > out.log 2>&1
来源：http://hz.jqgufenzy.top/gtjlobxbsz.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtijsvhwnd.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtphvtxjrn.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gtymjcanqy.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gteahzmnku.html

[R42] 输入重定向
来源：http://hz.gzhubu.top/gtudimqvcg.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtjjqflozw.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtmapvizgs.html

find . -name "*.log" -type f
来源：http://hz.cdnleiting.top/gterkdljyc.html

[R44] 按修改时间查找
来源：http://hz.xinyue.icu/gtrzdehymb.html

find . -mtime -7 -type f
来源：http://hz.cqqwz.cn/gtchttxova.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtftlzbtol.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gtkjflftzr.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtrburohsl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gthdmjxnyp.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gtwghefuwl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtrlplixag.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtqdrbpmej.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtbbswcwsk.html

[R49] awk 带条件
来源：http://hz.yj20258.top/gtqgvpghin.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtqhtnyqye.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtizescxsl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenzaomai.com/gtgvhmcwbc.html

[R51] 排序去重取前几
来源：http://hz.nwbrower.top/gtnusmsunx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenlongwang.top/gttqnjtfja.html

[R52] 统计行数
来源：http://hz.hammf.cn/gthffbmfdb.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtqjttqvml.html

[R53] 查看文件头与实时尾
来源：http://hz.jianghu66.top/gtqdywnabc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtoiyncduj.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gtrmkzmqtg.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtgwvgcblu.html

[R55] 压缩与解压
来源：http://hz.sweek.top/gtncvtrauj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtyxprjqnh.html

[R56] 远程拷贝
来源：http://hz.yuanzhike.top/gtyrbarzup.html

scp file user@host:/path/
来源：http://hz.guannengcc.top/gtyulzmaiq.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtxxwszpwu.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtkxdwzmyo.html

[R58] 下载文件
来源：http://hz.fengsongda.top/gtnpjochxk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtbkxgaopv.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtsdfbzomw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtdycmhuwl.html

[R60] 只看 HTTP 状态码
来源：http://hz.pycfn.com/gtdqhpmwzp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.havefunace.top/gtlojdpcoj.html

[R61] 磁盘占用
来源：http://hz.smart0.xyz/gtguuvdkkb.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtvsxgofop.html

[R62] 找最占空间的文件
来源：http://hz.vqdsnc.cn/gtmhlghbqi.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgfzy.top/gtvghvbuxq.html

[R63] 内存与进程
来源：http://hz.jinghuilouyu.cn/gtomxuhwyh.html

free -h;  ps aux | grep nginx
来源：http://hz.xinyue.icu/gtclzcqbvi.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtbhgqrtne.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fzhhl.top/gtgassaixk.html

[R65] 查看端口占用
来源：http://hz.hnxiangtu.top/gthutsvvgh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cheryme.top/gtxgobqoxp.html

[R66] 定时任务
来源：http://hz.ydzc1.top/gtuotdhuyt.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtqgjlpkzk.html

[R67] 生成随机十六进制串
来源：http://hz.meibo888.top/gtfpbctkvz.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtijlslslg.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtipthnfmr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nwbrower.top/gtztbpzmii.html

[R69] 生成随机密码
来源：http://hz.yvedp.cn/gtuomltltu.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxinkj.top/gtidwarajk.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtnxtznhzz.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gttoxmqkan.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gttcnmnosm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtyjjuovwc.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtztgsbrad.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuxming.cn/gtnlrsncks.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtvvqisjmz.html

split -l 1000 big.log part_
来源：http://hz.gzhubu.top/gtoufdpixw.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtgqyrvwqm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guowangkeji.top/gtjgzoqxrl.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtmifcrzyk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtaokpucri.html

[R76] 使用临时文件
来源：http://hz.zhengqikj.top/gtccwcrqjb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtotlcgscb.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gtpgtzgipz.html

read -rp "请输入: " ans
来源：http://hz.hfpthk.cn/gtjjvdgawi.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gtzvnsmzdz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtutescbkp.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtprgbdgln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gtxmhbfjbq.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtvedbrevq.html

time ./run.sh
来源：http://hz.smart0.xyz/gtyymihdwp.html

================================================================================
来源：http://hz.yuanzhike.top/gthjttlnea.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtexgqjvzz.html

================================================================================
来源：http://hz.yvedp.cn/gtpvsqdrvd.html

[S01] C：Hello World
来源：http://hz.zhijiandao.cn/gthucjyokf.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtwpwlxywu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gtslzefvfz.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtdmklwqvk.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydjk.org.cn/gtinmthxwx.html

[S03] C：读入整数
来源：http://hz.cdnleiting.top/gtbnzwrleq.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtyvkckcoa.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtjmsofidg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtkdcqjumm.html

[S05] C：字符串长度
来源：http://hz.yuxming.cn/gtvmavwnfr.html

strlen(s)
来源：http://hz.iojbl.cn/gtkqmlgyet.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtsuhnznrk.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtyqtsiywv.html

[S07] C：数组遍历求和
来源：http://hz.daria6918.cn/gtdlbmhebj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtnuglydpb.html

[S08] C：动态内存分配与释放
来源：http://hz.svipenyu.cn/gturwxmyvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258888.top/gttxqglccz.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gttqseofgp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtwtpdvgcy.html

[S10] C：指针与解引用
来源：http://hz.fzhhl.top/gtjjkigzkp.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtqwbnynkq.html

[S11] C：逐行读文件
来源：http://hz.yj20258.top/gtamwibwzc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gtnksqeexy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xuetiantiany.cn/gtywamzsyc.html

fclose(f);
来源：http://hz.cqqwz.cn/gtrvyzagkm.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gthyvuaxwq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fzhhl.top/gtcrgxzjqf.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtdzpxaxhd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cucudq.cn/gtwmpuqyrm.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gtqgqqnyoz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jianghu66.top/gtzropwcle.html

[S15] C：类型转换
来源：http://hz.shzxlz.cn/gtkubzybou.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtlcrxyalh.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtqxsuggvo.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtctvlcwye.html

[S17] C：安全拼接字符串
来源：http://hz.hysaishi.cn/gtxhjwxrql.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtyjouzmka.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtszixrgvf.html

int main(int argc, char **argv)
来源：http://hz.yangfankeji.com/gtwsbfpnqj.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtrzpbgohz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtgkkjklxy.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gtlqbgyoph.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gthwttehof.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtyvafkcum.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtbnmorrns.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtqfdlxiiq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtaplfsxgc.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtfemmuyto.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtwtuaagic.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtwswmjmta.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtumjvsfkp.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtkgnlowxs.html

memcpy(dst, src, n);
来源：http://hz.ywan-chungtsiang.top/gtseamqenu.html

[S26] C：内存清零
来源：http://hz.havefunace.top/gtrkffafqb.html

memset(a, 0, sizeof a);
来源：http://hz.zhengqikj.top/gtwkwegdvy.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtlyfdiaxb.html

const double PI = 3.14159;
来源：http://hz.aizwys.cn/gtleuhwcmx.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtjojulkbs.html

static int counter = 0;
来源：http://hz.sweek.top/gtpdranzse.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtjjpqcksv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fengsongda.top/gtugzlqezq.html

[S30] C：头文件保护
来源：http://hz.chenjidiqi.icu/gtwoyfujnd.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtnuojvlkp.html

#define X_H
来源：http://hz.ppjwa.cn/gtcohjhxrq.html

#endif
来源：http://hz.andypj.xyz/gtqrtzedas.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gthqrazndj.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtcelkebdt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtbpxuxxty.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gtrgsflhim.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gtbkaxyjoq.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtkkpndvjy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtpsrnkfkj.html

[S34] C++：遍历 vector
来源：http://hz.tanke756.top/gtgixejdrv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtjxctdksm.html

[S35] C++：map
来源：http://hz.shzxlz.cn/gtsbqihrwb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtlyeegryd.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtrqbgdkio.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtqigwjjfc.html

[S37] C++：set
来源：http://hz.ppjwa.cn/gtokhpwkmo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtbtngpobw.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gtaiadezdf.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtkbhnvjox.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtutxbdgsk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xingfuxueyuan.xyz/gtdfdgwkvt.html

[S40] C++：查找元素
来源：http://hz.jqgufenzy.top/gtxusjdzyl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtwwftjpwu.html


<!-- 参考信息 -->