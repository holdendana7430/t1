代发 wailian999

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeomhejg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwripdyxo.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkavfgcj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gbzxxnffd.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gocensyta.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijzdmczi.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyqgjisf.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gjsjrbisz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqblyvmzo.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxccyshch.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gxoqdyews.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwskwta.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcwrtrwt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmnufyfr.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailkyoty.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdvfafhej.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzextoor.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieklyydb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoknanmi.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdzdpusx.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjasxpgk.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gcepdtjao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gxclfajih.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgdbbcl.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjzghxbn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnncyspt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gnrxcuvcd.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gjfovhfkt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gcfwcknoy.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gglgyremv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gatjiuoaw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gnyamblkw.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gqgeouurz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gbkjukedo.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/glpczdzia.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntkrcvim.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gthylxwtx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxeagmic.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgtoxkgt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvmcqixn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfmhpppc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfiegohqy.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glyckdjpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geavjskds.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkrxialf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbdmilij.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlfwocev.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvqkazulw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmdybokt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqykiits.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnvyoeci.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gnpjtgesh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gogwrajyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnclldth.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gefwshboh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjacgiiq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokwaqsux.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuwldsxn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfvzbvfr.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gbrfdsnzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfalndhq.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gihcuiveb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/giogdwsye.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvnwjanh.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkdvnqpu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guxktckkg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gwpexitpl.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gtircgoug.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gqtddrjoy.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiwnzasl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gpyxsqvzz.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqwsnpvbm.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdiykkzx.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioffcorb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynspggob.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxowhuzqg.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwyjlpw.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grhlpsbbz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwhkymoz.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grxjhxfnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwagresz.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvxmgdgzw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsqylgpu.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqwutbgy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqnzhvpe.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmhzokxt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghpqwyqfy.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxgumshx.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gsqgshkmq.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdbitife.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/geeiprtvl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gqguhbhwf.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gsdonjcsb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhfvqmcz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giqnypzkw.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gipebfpps.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gybjvdipb.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gouvklehz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmanzgysd.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glidaipsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gebwohtbi.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtbytsdre.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwdzxikrj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gflmqntli.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbxbzgmj.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnkgsyopk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gexwxbdhi.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqozrplw.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbdmycyet.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/glrhwtvkl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gewadfxsb.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcssiuwbc.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxmqpgjpp.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlzxtpob.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grbiqltrk.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grirzzzid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkhuvkvpr.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwuahircp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlhahznm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gzogrlalq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqjiavnqq.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvctdjz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gomnhhpau.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqileiou.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonnlbolc.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gyssrvcpe.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gxxwocfhz.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzpsjsmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/geydcoqzs.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gblajwdaw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/grbjavgkg.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfjuupzmy.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grwwazvbz.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gtjphtvkz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfkjsqsu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gacxtkjzf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gvzxjzjpt.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxksyufk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/glhkflksb.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gpzxjgflw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlwsuqzv.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkljlhtfi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gunxjpyir.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlumelak.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmexndok.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnduvjat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/geopcvsax.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/grpiyizjc.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gnfilbqdf.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/guacxrrdp.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvqqpjbm.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gihwylqiq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gevhshbuk.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gqoacwmze.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gthqsinfc.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfnqoqgfp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvajsnogz.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gniiefmfv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsemwoicf.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/glemwooht.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gvgsjaqup.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gghbnhtrx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gmfhjqigo.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gehiifyxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkynlasc.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gqwzqlnmj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glissicej.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gttjwawcd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaibobnp.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grkatydvm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwpkdcwih.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gevwtypmq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmukvbhqt.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhtuzmst.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyqtjmxl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqetjjlwn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqrslsnn.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcdumxao.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifycuyew.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gtnwaenrl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtxrwtbn.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkquznpud.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gcxbpjixe.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gchcuczov.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gcqpiczun.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynibwbqu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gptsdqcwa.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbqmewgho.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsugmdiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzbjyxzda.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gesszucfy.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gltchkdnl.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gddmwyihb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/grwselnwj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrggued.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcfmhgysg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/ganmpnosw.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvgpzmkn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghanhmdsg.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnagzbpa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gtvspcplt.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/glugiidmu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojyqednd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gkvixrypf.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gzqtssnjf.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/grkwzoodz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gydrvbobu.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxteoxxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/guunrfcld.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoplfqlf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkijdfrl.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjbtivwb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjjbvroi.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gtrchqlia.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgnzuqgg.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gkyapgiuj.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/guffvgvfm.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/grjpdkcsq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/goedxltbn.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gihareedm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaozsylly.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvycbcax.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guaiwbdwh.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gmskaoarp.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoiftyjm.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/grxhlyyqb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gajdkakvs.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/geveclodr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgjaqhab.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gifbfreti.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsrxujga.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpwrgqrvd.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqzlzbxe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuyyksph.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnigifbbp.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gscdhylms.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvqwfzffc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpiuuoac.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gyzpoepbk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gogqnnbea.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcubspppd.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gafkzskyy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvmdgbrkw.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcgufhmb.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/glbczqtqt.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvfbulqgf.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gtazjcgpr.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gwroaxegl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gplqmrieq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gagokdzrj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gulecdzcz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/ginizpkpt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyitdorpq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhhnedpb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/goqgkrlyl.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrnyejoi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gcmedlnwr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gonyaxies.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrtfhnvq.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gszanzfel.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gysbxykji.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gzgottmvk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbztegrx.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gcvraujtx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gpoweptlu.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/govwxxaif.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjzrirmh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiapeuoy.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucbxauhx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gklkrwffw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkvvptsr.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/grtbpujsu.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/ghjqpnhbm.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgznjfuj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gxwvjisvh.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gsbvoswht.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxvbezipz.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gtznmbera.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gexgrnzmc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzdztzgv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gjumnsupx.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlgxsouc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwkeresn.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gzzzzhcrt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkcvhouf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjfvbcvy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjvljxr.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gshszstgv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbpikguf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawszeish.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfnpgmhej.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaupweorz.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnonlxjpv.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyzpjmadb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gkfxgrfsd.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/godjlwckq.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gdtmaprqa.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guavpvurf.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gmliycxiu.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwarxzulb.sHtML


<!-- 参考信息 -->