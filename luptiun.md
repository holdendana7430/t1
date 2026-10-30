代发 wailian999

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gymcggnba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gbnbidtri.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gofdtshur.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gnknixpdn.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ggxikzubg.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gixqsxhrv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gdwgqxttd.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gknxddiag.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gohjlvyeq.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/giirwcviq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gweersvsj.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/glgsbrses.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/grdpfhlyi.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gaetphpnh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gbhzqjfrj.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gggxwhtcw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gqopcvqww.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/genvnoedd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gslylnicm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gwkmxjhoa.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gbikywpdk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gnljcjwiv.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gbwupkowz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gjgrwbyov.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gazmjdgzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gxrpmrkov.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gqecgiqhq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/glshqfvqa.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gqmwroskk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghnfouyqj.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gsfynwrlh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gajziooqo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gildablle.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjdghvfdw.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gctaymynf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxggokqnx.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/grbfulpex.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdxltwmaw.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gqmkmkpfb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gaxphbxtx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gsrmxjwpt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gtxhongae.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/govlkiejh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gxhojdltd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gmmgzopcf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gmpnethha.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gowykwyln.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/ghuitqhyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gkslppsxl.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gdkvgcsji.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gyqqlvnnz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geyxnakkp.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/giwvukaol.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsexuekza.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gmavakwqe.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/ggtkmdlex.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gtfitnwid.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/glmimocex.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gymfilwhf.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gbersoakf.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gfizpcbqr.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gasttzdlo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/guebexpdz.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gnoczeyww.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gubnppiob.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/glhmyxfgm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gjhfiyrna.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/grsvjjqlg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/glurvysec.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gpgebktpk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/grnnufvrc.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnxanzgvy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnhkpgsdm.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gvgpfgctb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gloyvhjjg.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gtrcsirpa.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gveadusge.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbskkglmp.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/ggfbejsjo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gmaysodwh.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gimmsvegd.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gmnebohob.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/grthvwqdu.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gyjrthvij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gzzuedkxo.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gsxsbogxq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gnomfdhji.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gjqomjndb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/ggianiouj.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjbdyfrdt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gseygdfno.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gkizabomz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gmajvsnfj.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gfkbwlncq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/ggxqqihpj.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/glxglvwgi.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gywqcdfks.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/giavavrvi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gduazoonw.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gvotczufq.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gwwnlhzlq.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gvbjwerky.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gllzadkbf.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gdcloigyx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gwsktmmue.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/guntmfbqd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjeuiwf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/ggevpxzps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gbwyrckjk.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gnkujwonm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gwjfsrwul.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/ghyagmbtf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gydirkklm.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/genrnslrg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/glnjxixev.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gbzvwubml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gszjxadwf.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/grqrxwhvd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/ghohsfnsi.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gwrdytbna.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gyzyvscdz.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gsggalpnl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gncdlwqja.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gwvbcckab.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gfyinwhpi.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gvzjjujlh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gavaucacq.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gnxmqjndo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/ghdprsikm.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gukgbmcte.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gafxjubqv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjuzssz.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gyhxhfixg.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gocgjuflx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gyickhpzn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gtlupplhv.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gpiuaouxn.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gttrkmcyi.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/grqlwxdzf.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gjvqacxhv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gskmicyiv.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gsbspizxh.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbgrjwdon.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/ghyvdjaum.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gjuywrmxh.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gajzydfcd.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gwhhmwbcf.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gxqnwjfos.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gyniajaqq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gmwkdxzep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gleqldvuz.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gnskfkice.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtnrgprhi.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gaippzjyn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gofkeewdp.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gotbmwaog.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gfcyixvmr.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gknbqqbfu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gfhokkqsy.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gqatcbnht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gvyesdmcp.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gnktxcqom.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gujcifuyq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gtqekirgy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gonykznvh.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gtzrfyawm.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/givbcxpic.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gemnnvyvl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gppsnznev.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gujidpahi.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gfofvonpg.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gltpujiim.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gidloulqt.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gjfpdlghm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gbjcmzkvt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gvzgortll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gjhckerch.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gmfurbhds.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gkhxavjkb.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/grskxmbau.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gqpagczhe.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gxewsvxke.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gploboqiv.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gozndmaqb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvpqzyxcs.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gkkyogcqu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gduokftsa.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gpozepomw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gffhmxlqk.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gvuhfwvbv.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gtzvouqsz.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gcfknzijl.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gcvtrvjbz.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gyyxexqhz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gqzowencv.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/glmzplmkf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gmlomfwri.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gccbemniy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gchiphhcy.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gvyxvtjvy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/geennupqy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gccobjahn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gsrrzbklv.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gziezndeb.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gczxozygz.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/giannwrxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gfhgdflyf.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/guizdnorn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gabswutxi.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gjupuciqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gcdjkxtmf.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gcufupbmo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/glzrxngey.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gddejlvtb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/ghblrfhlz.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gyfnthdkx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gihvhmfxi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gnpuxptjg.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/grmffbejt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyxdrvpnd.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gdnvvozot.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzcdlksde.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxmbnvekj.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gekmrdzxf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gpkfwydjz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gsqqxmruv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gduabbiig.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gwxlnyfyw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gibkihacg.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gnwdnjyor.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/glvsfcokw.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gypynjdag.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gkkmmkymo.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gflbkznua.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gzbsdfoub.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gufvabfjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gfelruqzb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gaivrscyy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gipgvvlbt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gxatvjkyg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/getbpkjhr.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gtpvaplxt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gbvbystgx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grljlvtnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/geaxuqlcn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gqssjuhou.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/glcgyrkfk.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gbxcjauut.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gifczwkhn.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gkovfhknx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gqvppufpi.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gevquwnpg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ggxbvlfuu.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gxcmobjxb.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gmemioqdr.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gdavwbrmv.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmnfwmse.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gatvnffwd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gjzeakckd.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gydbmiycf.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gkxobndxm.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gringzmal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gutwlzieq.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gevphrfly.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gepxcnemz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gqzksvlns.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gixbcrvwd.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gshbyxfeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/grtlulvkk.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/grhgyddzl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gwmqobaqe.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/galfyazrc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gobselbij.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gsktugjut.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gusvbxmzx.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/glaepgpuj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gdlcdkrux.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grqfpkiov.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gvaebthif.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/grfttggng.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gkjqcmpdd.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gqihkewri.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/geelhirns.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gmzoikpad.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gvceahaja.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/govtnhswf.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/guvraivsh.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvdmpctsm.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gogbtcucu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gpvphakpp.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gcvqrfsvy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/guzftqvxh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gxkasqyuj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/ggogxtuxq.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghdaallhb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gnkbqueyj.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gquszryrx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmgapmxyi.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqjgtjhvp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjvsxuhqa.sHtML


<!-- 参考信息 -->