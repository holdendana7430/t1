代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gsxjpmhwh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gxqjhrhcm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gwxsajdrv.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gsjqgfrnt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gafwptsrr.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gwwmlmcvs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqwwlxkyz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/giprjteaz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmzgmriob.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/ggpchiknz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gfbcwctqc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnvndbmxe.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gawmxrpgn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glgbpmwkm.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gjmlhjnzk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gzjkdgexq.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gskrzxbii.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gautwsozj.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gvjzsfzgd.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gijzzgsge.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/ggklxakwc.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gudyhvjtg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gewphgtnu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gtcqmkowv.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gquevhteg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gnkqjmwht.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gotutpzdj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gttvirkyc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gwwwklfwf.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gnpmachfo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/ggtpnoqjw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gawvtrifi.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/ggdosmumg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gobvlonta.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gkoxgnhte.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gyxwgwdyf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfnpigowu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gzpwbagps.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gyncxdqyu.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gbazhgndr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gfcmodajf.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxvxjganu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghsggfmxt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/ggwluzexb.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gmfutiuxr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/guwygndtp.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gvxqhlvnh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/giqwvualj.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gthtqnejg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/ghvmfmbnr.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gvyfspfkd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/grgpzqgub.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gkalnbmhp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqxceyqmr.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gglyhfpke.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqetzsmle.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gogsppdja.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtpzbpikz.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghqtfsxyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gxqqopahg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gphnaxeka.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/garxvjhhi.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/guqmbmxkv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/glblturmk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gmmgwtsxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gkktllugh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/ggowcknwo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gyrdmrqiz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gomlcbbcb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gtlgifcaq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghnnqgyjm.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/ggwjmqhnv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gnzngubpr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gctghugzj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/ghcioqyzf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grpgxujof.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gizvvcdah.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggnjfbljt.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gkjefvwft.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gyubzsasm.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/ggspsockq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gpcarqtxr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gsjuqgivo.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gxbptdlvb.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gykbbglcw.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gziifoucy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gvhfstscw.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gcgaynqmx.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/glogzqfpy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gevtpfjdt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjirfsob.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gopvnlsrc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/ggkksqgcl.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gzbunlfki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gmcxiabxj.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gyasmgpiq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/goltbdbuu.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gzhkxjnjv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gfmontytx.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gfrhrcsth.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gkkxpsmsh.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gwrnqcdjj.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/glfcjgyzq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gtfxsxghp.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gjzoxhhjn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gcheqduqc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gkuudssap.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/glfhuzphg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwcdcavjg.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gbentgkaq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gclqhxywg.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfiuugppz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/glpajmwrv.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gfhmqzqiz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gxksvdees.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gsbpwgukd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gblaxkqvf.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/guxwshgbj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/glxcodaxv.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gjddhigrd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxpdczmnu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/giwuptncw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gwokkoyaf.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghqxlvpcd.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/galzzqymz.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gycbmwjyb.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gwxjkzqph.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gkgbzbwmm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gbxhykhll.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gtrzunzfw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gckykkqrk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gtdurptmz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gdfxlysal.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gwmqoknym.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gejemjohe.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gcjyspkkw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gwqpetcwu.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gbpxspspt.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gmkjxaisl.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gpbqsgybr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gsblbztmw.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gvypgqyug.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gdkstzsmw.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gdgyitcrf.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gfifstblc.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gtqecldvg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpquepld.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gfvruhoqe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gafmypflt.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gomufkqln.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gbkhcxboe.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gchdmflzx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gsofmyodw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/goivjysim.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/ggngtrjuv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gusdnfqix.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/ghnrdelax.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gcgbkhcsq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gpnktjokt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gptkxogcz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gkpievpxf.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gajnfsaff.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gqdhmzfxw.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gcjnfwhoh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gowehphoo.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gdtgoknhy.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/grlrigtgj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/ganozzwcc.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gtbitvtdd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gibzuezce.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/goklwnbbx.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/guaxunnje.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gfxoedfgt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gyokyysrw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gixyyommg.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gmqhqwzdi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggwjprbjc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gnuoewdzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gokxpmljm.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gcoohyrqo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/grwrvlads.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gsodmettc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gvexkmowq.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gxlpzndnm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/grpjspnhj.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gyypttujd.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghlookdqd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gphigrlky.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gawswlpna.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gguzodlzs.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdhtxrcle.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gfmwigaen.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gnfwbqkpv.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gjufwlklk.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/ggjeatalo.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gtecjttmv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gnsffjytp.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gwrwlnbvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gojojzlse.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gspphbfro.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gwhqaqbmq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gsppqklov.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gqsivghke.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gfdclzhpf.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/geukatwcg.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gkdgnzapc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gwkxfmrgb.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gvinrbpre.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gmkqvaecn.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gzqshbvbz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gciyllehx.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gmqneawdw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gtxjmwxqn.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gjftvvkyx.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gigrryfur.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/grcqfvfiu.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gbwkpcsbn.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gnmfgzhcy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkxkhjvcp.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gafwmirzv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gcxsnorrn.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gzwllvius.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/garyeckkb.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gfxwcfspb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/ghymzvevu.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gpcpmkjsw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gdniitjfi.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gomugnhqg.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gbufkhxwr.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gecjrrjqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gvsntqqtz.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gbntwrers.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gadtisdjp.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gavdjownw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gdycgihpe.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gahxctetv.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gtnkdexzf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gbcwprofg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gptsbyemk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gzggbprlp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gkkkayzwo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gycjunojn.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ggbbsroxy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtfacurbk.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/guzsqpste.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gopulsumr.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqwlalmhb.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gbamuvick.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/guynbbxhh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gcasbhrwt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gjmwrgpzg.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/giuzqdoje.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxvtvbo.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/goxugykbk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwdevcstq.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/glvultoma.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gjenfuekd.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxmflzvvh.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/glrinaogi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gorzxubph.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gxxlllvut.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gilfjjimn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gtnibtpmw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gdfvtfgog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gtxfaatir.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gyagtwdqb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gvyhoduwj.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmkmgetay.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/glsdthlpu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gkvryohgw.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gfxingbjv.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gggannedh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gkhkihtbv.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gsuzzfjsx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gpomhpxav.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gqntudvsm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gilaszmfr.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/goeixzose.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gqjzywpmi.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/galyoqsut.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gjwembfup.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxdwyklec.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ghtltjcco.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gmhgajwpn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gywuhxwet.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gnjtxvaua.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/glpxjcnyp.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gqgclllig.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gmkdhpcxn.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/geiszqjdw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gtkvjjpsz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gjpnadfai.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gyituxicu.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gkxjqtkza.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gqtnuqlkv.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/glgqmmrcj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gptoskueb.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gjfgfsjmd.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/guixtoexo.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gsuiwknak.sHtML


<!-- 参考信息 -->