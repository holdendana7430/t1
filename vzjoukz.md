代发 wailian999

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gcaociduk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ghbykhjls.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gymbdoakd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/grhgtqifg.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gnijcmqvg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gxbgvcani.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gzpeycmmx.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gdzphhvuf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gaajfqdho.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gvscdkosb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gywxoytvz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gcdxnpsta.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gucmbbtxl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gkeyxqmgd.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gpmrvrwcs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxfhwrzgr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gpxdsyrfo.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gaiuhhddl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/glkoobjei.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gwaxwwzvg.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gntscrfyc.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gciwkrjfn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/girhqepoz.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/grvdtjtyc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbbwbblqo.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gnpivmtac.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gvprezczy.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/geadvfzfg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gambaxefb.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gotczopvp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcgwvcfix.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gudrlrrpf.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/ghjodvrks.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gbtyeguno.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/ggfkbvosx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gwvbtidyh.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gjzrhfvud.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gbogpegik.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gwlfjfaxa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/ggtlrhudn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gtgpqegca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkcvjkoqn.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gsiyfizej.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjtmiryza.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/giddlvljk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geykecynu.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/giricewug.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmzfsgegk.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gcvwklyjr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gudnwgydp.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gkaohdddh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gfoljxdkb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gcvnzljuh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gmisxeawh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gqcjfnhih.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gyoasacdp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gwzcnazch.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gjbzkdgym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxuhhsspm.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/grytxlite.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gojpdujag.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gpakbgdwl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/giejbsgjj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpoakfvbx.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gzsuxjuuv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gayscqadz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/giqjdgmls.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gexjbeoeu.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gltoolcnb.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gfbzuesiw.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gxgvhrsdp.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/glaasmjbx.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/grdgfzvxl.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbcissxid.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gzofxmsuf.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gzokqvhac.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gzjelknbi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvjdyrcpu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/glwzodzoo.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gbmdfwigv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gjsemhawh.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/goelfkrbr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/goeqvrqdr.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/glnqjtnao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/geueivjur.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/ggrstzarz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gessklqpq.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gswmmdjhq.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/guorpabcx.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/ghakfhmby.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gemfdsatm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gbblcqyzn.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gkzckogye.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gpztksqbn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gfvomgnnv.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gzjrphris.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gtktycxwg.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gmsxahvgd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpsakknud.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gortwwtdn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gguwykczi.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gljlhgvvu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gvjzfluqk.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/godzmtlnb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gtbwlfdnr.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gonebhbzj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gixzdjbvc.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gqehoetcm.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gjwhlhaun.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gbjryyouc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gmkezscnh.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdfkqungv.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gvnawgjfo.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gorldvirc.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gxrzsypoz.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gmkvktcti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gcqwjrrxs.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gohhuizkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gphmwmnge.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/ghrykndmc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gqpikiutu.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/ggvwqakbc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gcnztvezg.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gccoslaoo.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gxpifdvsk.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/geabjtmdo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gewfhxjfv.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gozkctzlz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gptrauati.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gnkrqvmil.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/guygbbzxq.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/ggdwlvzse.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gqjmjqdnq.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gtdsvsduc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gbcdqpcjs.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gbgwzpbkd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/grkplsbqb.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gsrmmigxb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gegjtwijl.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gkqnluzue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/giceullsr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gntyxfseb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gnofajpng.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gckuvawqf.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gmlzkulob.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gfzbvwvoa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gfbausrwm.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gizrmsnbl.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gtjozmwck.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/ggbpkeoiv.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gailowfci.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/ggyqrxyib.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gdnrhvdkq.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gocpctuns.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gjtakosvg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/guqcrwohm.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gaefwirdj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gdgthspwv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gwzzoxiyw.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gtcaccdln.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/glogeoxot.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/grbzmgbcr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gkusyslic.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gdwdqphup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghxzfawsb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gzanucorr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gsckqmglt.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gldqfiluw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/glalcclzi.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gcyefiznk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gfwohjeqb.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gfulmylxm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gursapgso.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gbdwkhvkj.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gligjqrla.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gkmwyramk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gcakfinmd.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/ggqqlsjmt.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gimeygyka.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/geqsfkusw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gxolvcdsl.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gmxfmwrmc.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/ghqlxfsmq.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gwezireqw.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gwguphhjv.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gefnfyari.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/ggedvemxt.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/geefqzgld.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gdkktpgnq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gikaqdazx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gbigpihgn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxwilvvmo.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/glldhpxgh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/ghwbbbzvi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gxglrsuih.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/glgfajldo.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gusbffohc.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gflkuferb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gpeiiszkz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpxxmlccd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/guvvfjzuv.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gtzmtyqxu.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gcnlzlnuy.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gwnauvxeh.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gofkunxxh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gdhcvbenb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbhvihssw.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gwjpztsjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbnbssp.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gnzmjwfny.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gnhwcvdkl.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxqsruusi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gotelcipb.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gwodpaokd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gveoubeum.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gyaneymxe.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/geqxvkdrm.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/glynuxjzu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gdqwjaivc.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwwlkkpjo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gbrqgxvah.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gddbihulr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gghtebpyx.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gycknhbxt.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/guffyibux.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gnnviytng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/ghpqxrgpf.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gsarcxrtp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gdlglqact.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gjuohoshd.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gvcllgwmj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grxlfwxfz.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gbdpmkkqx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gecnsfriw.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gowutpbvb.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gtvdrjseb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gkuiusiss.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gnwmmqneg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gdjzlikri.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gynjnadsa.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gdaeuxxqa.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gdbyiuzad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gqogghusp.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/glzyotdse.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gdoxrqvvr.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/ggjqpjylv.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gqazoevil.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gswrianhs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gtemlbqrh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gsjedsosu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/giwirecqk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gwqnbtiqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrhlxrj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gzehfgsdc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gqnrenlti.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcqzeelin.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gjbzwtbic.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gkjjmbhro.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/genylqsxt.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gdzdrwjym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbgkqttyq.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gdxghhaor.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gxqwksqhw.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gkvlhjrqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gxswqczwe.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/geqvivvot.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gunbvxvvs.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/galrexcnt.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gndbzzanu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gkvyvdhmn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gowsncsro.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gcfkywnjs.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gxrtelobd.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/giiubzxwd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/getyaxjhm.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gfbsswssl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnwhfpgit.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gtyxruhmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/grnldbfig.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gyyoxfadx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gxdmgkxcx.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gvalzweij.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gwdbvgcle.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/guonihsfc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gbrwkjagd.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gleanjjxx.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gcpebqdap.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ggdbbdpva.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gvvzztpmk.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gvkxjgldh.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnovfzxxt.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gabitprdt.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gqaipfmga.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gjarbvmyj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/ghngsfqvr.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gpqmgelxz.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gtcyhoyku.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gfhkczgpi.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gpvosabai.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwrgagnip.sHtML


<!-- 参考信息 -->