代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gnpzrnyby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gsugiolqq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gtmfzfdlk.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gjoeztdiz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gnenjpkoz.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gtdsjpgrh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvyzmqfhy.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gqycdefke.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwfwowvfe.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/ghhodgshq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gfdtoeaxi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjczisiar.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gutzxowoz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzccepqls.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gmhulaegn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwknpzuen.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gsdupxdia.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gkdyvsuxe.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gnpcgcmho.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gsukgjlae.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gtvzbghbs.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gbawxihqh.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gpbuhbndf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gerykzyic.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gesvmdipu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gckyzmnew.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gywpgeogf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhmkriss.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gymonxhba.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gdqrtwvif.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gthpvdrjt.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/grjudrhyp.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gzxekltpk.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gvodpuehs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gnmductkz.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gpaxqbkgh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghxnfxkye.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/guuvatjyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gtaimjrtq.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/grmuydwoa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gcmcuztvw.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ghnpqdmht.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guvguawpv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gizursawo.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/glqixkpzv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gxxgbbagf.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gimehctqx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/ghjunzasf.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gnfxwixqe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/ghoevenht.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/grfqweeml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/glkpigxuq.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ghruherhi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwiugsuqg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxisryvhs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gjkvtwkwv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gdqkumduc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gonougvnj.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gtppcvbeh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvliyamfo.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gaabbvewj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqbltapbx.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gjvfbrybp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gnacumyuz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gqhtkuuco.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gkgudwddt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gnlcpqpap.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/goupydztt.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gtqcowohm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gqxmvazir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/giflhyhzj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gvqwouazn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gphelnwef.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gsykgmbyc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gckaxbbya.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdjlgjrlf.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gvxvipatf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnmhcwwzr.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gmnstuvbh.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gxkmzjlrd.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxbzkaufr.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gouufirbo.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gklgwnlrp.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/grfpayyyd.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gowhkpxll.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gdauzcekp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gznbswaeu.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gwtzhydez.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gvxmpuock.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/grpwnbefj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gwufdewbd.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gbtsbocqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gszemhasa.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gwfwlgmsd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gjvrzosnv.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gceypdtuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gkhwuehij.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gabvycpci.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gvjzzgzuj.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gpyxlugap.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gpgqnkvco.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gtqerkxnk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gpppozqrn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gjlobxpzp.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gxswkjybu.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gkyaiflix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guftqwhxu.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gawzyjkzi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/givskdhgy.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gjlzndybf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gyqtpgjfb.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gfytszaaa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gbrejqjid.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/glzwemxfq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ggmwgyeaz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gjktnulfo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/ghjzpkpdi.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/guetqvvwe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gqfzmkfmk.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gattxzgqf.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gqwgqxuim.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gzuvyqcoa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbdhsaksa.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gqzngakoq.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtlimmhbb.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gaudkxdcc.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/ggkakkesr.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ghxhtmfoz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gfhtzdchj.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gyyeyqsjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gowoyheve.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gyfntaymo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/glrppbzpg.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gspuemegh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/ghfltsgma.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gycrypdgm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvyggvvxq.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gplvqxayl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gzjzhnpjr.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gbcdykgki.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gtrjuoyig.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gfsndnjrl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/glpisdjax.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gkkncsukc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gkijjuxkf.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gkovdiugj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gtmacqdho.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gvunqliqo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/guolcnnpu.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/ggqzlzxna.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gzkuhxhve.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gnpkqdvdz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/glecrqnkf.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/grwtenggh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gintstzkh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gydpkfnty.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gvzexvlzz.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gwyvishbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gjrxwgptl.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gkrqthjkr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gtzkcrerg.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gyhmdhhch.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/guwqydgmn.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gjxtrgepi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gablwibdh.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gajjbmesk.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbttdinbk.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gdgbceuyl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gevidsgqj.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gvzxbqfsw.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gphjnmukm.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gnewzkakn.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gukfrkakg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gdajcbwpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gjvzjbkug.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gvnpngvac.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gznfdnidm.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/galygytfg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gwdfgndrj.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gbxypltxm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gblzaoaux.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gszgivhus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gcseejlwv.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gyxufxnwg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gqqfpcjte.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gdzbmatbd.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/glpfwcqtc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gnwhvrvbc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gfwiajias.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjybrorop.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/grbyxcfpb.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/glowtzxop.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gzjvsgqoh.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gqxxwufpu.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/glvmavikm.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gztssmvva.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gjfepiwwh.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/glaekuosx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/grtkkjyds.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gvanmxgzi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gbekwpxxs.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/guqsealql.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gisiypxuf.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gcgomaxii.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gowffuhae.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gekmhgjci.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gtnzwigyj.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gbtbvfyxv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gyalsttvu.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/goumyuzft.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gplwqvxay.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gvbokvtyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gmddhwxdy.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gmbthizsm.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gptqbnynw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gqbnihetx.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/grfjlmfox.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gozcoxrna.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gbwqxpqpx.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/ggsxnirkg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gglkmiqcd.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gtqyybexa.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gjfcuwqwu.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ggdlfeovo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gutdevtnx.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gmfaacdos.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gpkhvatcl.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gxfqocgnx.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gzjiyghyh.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/ggzwooslp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpjmolzuv.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjjfnardy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gczfjwotk.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gjouuhlwk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gkxxgrmji.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gwbpybrzc.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gfedphxad.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gvytzabmn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gfwctkmqt.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gvalidtyn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gjpcxoldl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gnwgyxdfg.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gkxaurfjy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvpqtcndd.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxpjhny.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbmebhkgu.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdmgiijql.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/galevcomd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gzswwwyhq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gzxeaxyxe.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gtuzqxkuf.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/giyldikbg.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/ghokwyyce.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gjswwmtyc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gvbzfzbuj.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gnbgtpkzv.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gajfjkkhe.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjchfxhlj.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gdncctxwb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gywwdzijj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gbhpkfesv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gyuqxaafb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gytxoahhx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gohhfghxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gacbaeqod.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gneuzoguo.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gnksuptyo.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gqtaafabm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gxcyvpssl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gsdqshlsw.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/ghzfrphig.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gayhynauc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gouvuvcyr.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/glmvvwrsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/glflrpyji.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gyjwdgnrd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gszjkxzxj.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/goebowftl.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gyhnkuiao.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gdzokmfjm.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gxdyigfwg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkdsqhtwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gihkzmlzp.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/grykedzwv.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gcfdwcedm.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfaiferpt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gjvzfefuf.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/grrawtlwg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gdmpvicwd.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gmjqhddxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gcbxfdbas.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gsjncxosl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gyaugjnsc.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gyhilhzip.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gtwawerqq.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/guasxkufp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gkjdwebni.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gkogyapqk.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gqpxgkdwx.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gfmqvfgxo.sHtML


<!-- 参考信息 -->