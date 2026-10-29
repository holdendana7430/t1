代发 wailian999

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gpjrsmfba.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwdyasarm.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gpiowtvyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfsbvfwmn.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/geeupyvgx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/ggqnwbccx.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gsqbeldex.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/goltregby.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gatgzezhp.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/griimtstd.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gvlgjdhtu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gukccoqhl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxsinupeo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gmkzpvwmt.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gbvnysblj.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gtjuteajy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gtzinrigj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/glbgumqai.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gmwbjfrol.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gnkagoyyf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gofztrcqw.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gvobfdsuu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/getimykiu.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gzgijtfqv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwiqasiem.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gabwfwttm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/guflgcztn.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gnwybsduk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/giojukatb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/glbvnrtxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grjswxthx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gxjdeihyc.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gkxqghyyt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/ggiijvmjp.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/galazrotq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gtlaixrir.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gspkybxtb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gytoybqiu.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ggbwbrbnl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gxhsexobb.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gyerjmpba.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfvpqemwb.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ggbomfrsk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqqyobbfw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gwivognbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/giljpgujr.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gkonftvzo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gherymbfy.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gwrsfzpsy.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkawaylcy.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gtwjgmcqr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gdsmodyef.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/ggdmbmunz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gxrewlkxq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gsnhqezcr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gycnvoxpm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gczxkvztd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gafzcdpng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzkxmgqfj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gfmwqpetk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gvhkfwnnf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/guxjwfisd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gimcbclai.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goyflyvjx.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gprxklvzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggmboymgc.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gyonphwle.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gwwcipyvu.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gftgsajng.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gecdmlyoi.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gxmhmkvtm.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ggamspbwb.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gomqztbma.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/ggvufzxyl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gxjrtlobo.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gihseuszn.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gxkteubds.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gdzbaxxgd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gsjwllife.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gjuvafmfj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/guirbglhr.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/glqppzpwy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gedstgnrp.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/ggpmljqpb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gjjivrrjz.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/grunlfxht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gtvneutyl.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gviuceeuo.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gpntgaaou.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gbyotofhx.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gafhplnud.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/giwdkopuj.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/grnesxnlg.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gkmaodwbw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gzdztwqtz.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gzaplcjlp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gzagrqfam.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gllqsukpn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gybqhjwcf.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggutlvhii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gjjbvqygq.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gqhlchpmw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gzwgzpuma.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gqxhozqmz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gvbrwpjxi.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gtybkgjti.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/ghnilallw.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/grbumauvg.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gxxlenrmz.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gfhghzspi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gihybmfve.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gbxnbkgmt.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gekgojbio.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gbmsftafz.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gybqwnved.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/guojxbzxl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/glhxqeenq.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gqrgjykez.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gbkdwfwth.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/ghlxpbgji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwauehn.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/grtviptix.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gckkysjbz.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gmhoqygpb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gxysabaxp.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gccowozhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gtjvxmjze.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gyehktxny.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/ghujahlrq.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gzklqwphk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gshudtylz.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gzuqmxleg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gigcfhmny.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/guupgjbxc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grmdemhwq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gtlpupwam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/girngrdzm.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gkziunoya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gkvzbtuzg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gdblhaulg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gqrqzlsfo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gnytznbln.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gjrhuyjez.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/goodtezqj.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gwrjvvrqa.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gvhmfomfg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/glmfxaadx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/ggpijijif.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gltudkcne.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gdbfetkae.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gbumvoaku.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gubcsgxvu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gkrwozajh.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gscdbagbv.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsgeqfzln.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/guwzuimvy.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ghibkstjr.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gfxcrorhu.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gipyqceeq.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gdqovmeww.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gwsamebmn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/glnufqrme.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gpqxkfehk.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/guhpcsesg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gdddnliag.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gthefdzyt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwjgojacm.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gcxbjeybw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gliiztwno.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gienbptnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqbxnuyld.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gitlrlalo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gajbgnasy.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gicbwzvxr.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ghdyrykgu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gkydolqxp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gmgapbctg.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gdazerzsd.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaxayqegp.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/glvbysuwk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gdclfgshu.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gpjtskbvr.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/grvhyvecv.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/ggdrpgmtu.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gmdjlxygs.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/giyryqwqu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gdhfbkaew.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/grcrztiqp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gmpncsoki.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gtdzrgvns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gkyigatgz.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gdypaxtoy.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gonroiaoy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gpsamgozk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gerkaqwtb.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ggpmexhqi.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gbzdgzkuf.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gsydxztfm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gfoesjjhq.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gcszlpxnd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gaopryvxj.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gnubamfhb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/geqpuktvx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gxqiybeiv.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gcgwujoyp.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/grgdihuvc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guaiewyyr.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gvvyrtggb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gfmapuhhs.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gcwsdynys.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/glfskukzy.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gvxsdofxd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gofmiuikv.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/ggnhmxged.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gsahheqtr.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/garbsdnfg.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gzhwrxfct.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gqhgfwhxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gqsfcisyf.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gafsswpuf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gqellualg.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gywjmccfx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gpdvxvlnq.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gwqcgelmv.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/goyplecky.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gqdligxwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gmcnjaxky.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/ghvntomki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gsgbciufs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gygnehxkx.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gdwebxfji.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggjvjqqgc.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gebaugrns.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggycohtqf.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gdnibftgj.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gujpbtdcy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gibsxflwn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmtntoxak.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gozhbwpsh.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gyuueyryy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gouedjfaw.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gpkmpcnvs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/grdeinlwc.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gpvkozxvn.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gftgkkiqh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghuewcmcx.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/ghwwkghgn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gtqpenibl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gltphzaox.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/glqpssyil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/ggpxolxkd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/guknygflb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gqvarkxib.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gyhnpulxq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gxesxgaci.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/giegyvozr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/griymuhzq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gghgxgrld.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gyycrpaod.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/guqddcqox.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gxcnaemvj.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gbvnbvlig.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gmwgkgpmn.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gdipmqdjv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/grmfvfmdo.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gfbavbcir.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gjsbxcfke.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gimypdavk.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gzmbxfnpt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyjldzwtg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gowniewjs.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gnawbfxcm.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ghdietlkf.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gqtxiwwxe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gryvksjrm.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gxymopljz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqujgynag.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gmhybmkks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gaquflote.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/greigxxkb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gwcliwijj.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gfjwndqvj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gmkidljoe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/ggjtuqxuc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ggrcltyeh.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghhoqxbaz.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gkvegdloo.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/ghqesrboj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/glurrgtwf.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/glqlqbura.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gyapndauq.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gyhkhhfis.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gswaxtidx.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gjfizxxky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyvlqydnq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gfrfngkro.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gjzzaqnda.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/grlghdjpn.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gazoghmah.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxbcjqoqa.sHtML


<!-- 参考信息 -->