代发 wailian999

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gtlczvsde.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gufbumqui.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/guuisjrmv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gjnemrvmg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gaohzzvvy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gxnsoijjb.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gkcykgotc.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gojfzzcre.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gdxnubfqa.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gdlotimfp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gvubeubbw.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gcjydoucn.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gohfiyrwv.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ghrnvlsfm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/givvdzzdm.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gxvjcaitw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtbevuvdg.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gtyxumply.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/ggmpvcbjz.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gkxrkcqkx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/geocvazuh.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gehhylzau.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqpnnhfej.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gxlrtqniu.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gxbkppmfb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/ghxmqepbr.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/ggyxdqqgl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gsjsyumnj.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gjkbeltcc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gknlstgdn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/glrtosmfl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gtsihzevg.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gabiwajdk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxuvwgjzm.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gllmpcraw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gqqsybpsi.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gjpwafkai.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvvxgyqkj.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gbxactyhh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpoarpmqf.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gbfwvfwrk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnxilbwdx.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gvlikjloa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gpajcaqpf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gfhkkfcfl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/ghltgxygf.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ggonntcjp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gydslqocs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gzydpneej.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gtkfkdxma.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnlpvwakg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/ghcwwvqoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gbxoztibz.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gszxwtivq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gtvwrskbi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glknlszfg.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gnxrhpzsz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gilgykhmd.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gefnwpkbi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gtnidklwf.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gwfhbryym.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gwnfkdgva.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gbxcgufhx.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gdkeqpjrj.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghnhkqrmg.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gbfbgsdit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gxvmnihck.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gnaixyqjk.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gfmztqrzw.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/grhydbryh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeetwwqm.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gyjmbfpmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/getnblync.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gmlfqmska.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/grabznzga.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gawmxounp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gnupxifvg.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gcftzluus.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gjhxgzrro.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gtbliuohw.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gilgiqzns.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gfdrlpqom.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/guenxnwxv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghlxfslco.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gmoshzpxp.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gvdmenzya.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gtesedepz.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/geapwcxbc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gmcrnxsbx.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gcsnrxfep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/glhansihs.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkvujhtev.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gbhtrwptd.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsdjbbako.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gpvzlpkvz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gnphhtkyt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gxmngatia.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ggxmgsxww.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gsrkiujbr.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtfdzimvg.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/ghcdnomoc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/guajjeuxc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gkqgrgutp.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gbzunzajy.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gubxrlatd.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gqdykltjh.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/galrseofy.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gimpzmskf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gwzdyhhff.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grleggikr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gekreboyn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gbssmgzbn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gyaewesed.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gqmuidtmk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gzjcxoesy.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/ginvcreqr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/ghweumkfi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gytqpoojf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gkpzltlej.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/ggwfhlrcc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gnmufyerp.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gfcxqskda.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gyclqqgsl.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjupasjve.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gogmdozjo.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gacgiethv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/guogsjwtj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gqifxoosv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gytmsmpiw.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gxbvmuyyw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gazxclmnz.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqfqjaw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gzqucogct.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gjoqxanow.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/geznmxedg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/glbynqcxk.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gacjhetmq.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gjesxgmnt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gzxmthzgd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gmemcabzg.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gykvvmtzx.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ghjlkyqoa.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gfufjmaiz.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gqbvsfpmk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gkwsdqzzs.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gnqibfpwc.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpgtjtexi.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ggamjnpvt.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gokixflin.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gpdhllrbj.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/grihcjpzj.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gtzphsavf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/guhpwhtba.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gjpukdfln.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gkibtjvgc.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/ggpyjompt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gdngjxcpw.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gcimhzicq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/goeiprdsw.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gfwnajktg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/glpyfsweq.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/glcsrqiju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gclkwscat.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gdcrbxfxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gelcsgflt.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gfzemcjrj.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gvrsszqbq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gaoqanilq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ggkxmnyth.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gkkqdypia.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gfutujshm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/ghywjxotg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gzsghwnyt.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gldzdkfet.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gxgyjgmes.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gulsplneo.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gulpdyoqo.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gbbsxkamc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/govpidtnd.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gqjzgcikm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/ghkanqqbw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gqublcdfa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gubvxaegu.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gqmdpunwg.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gxumrpexo.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gveihwzrh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gdutpzldl.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gpwzblnrs.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gscdxwmit.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gznnjdadm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/grxqcwxwf.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gsquqslhe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gfmvhyngo.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gbrdkpvzz.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gkhmisvty.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gxumtahtt.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gefljtbuj.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gokovbrtp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gyijmkcjg.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/grkcohxck.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gooqhuxdt.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gmpsdmeru.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzeopdf.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gytdzunpw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gvxpvwolf.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gedzjhags.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gctxkgkjv.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gdjrqlqac.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gokujttbz.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gltifnbdv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gihlqmzoz.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gdlgicaie.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gcipwhmwg.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gnxukycsr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gsvlvtslx.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gkbtynhll.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gmbgmlhbp.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gwiblplrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gmhipabja.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gfiznxuki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/geyctbscy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gukwifygm.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gkgptzdff.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggzplifzc.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gdxmpiktw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gptrapmfr.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfqtwgqsy.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gocdxqaxp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gmryzboqz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gywmslsoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmrcstm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gqumaldha.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gfksvqrel.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gecvtrfej.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gsrpegdui.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gtxemmbtv.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbqfuwbfn.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gdcojjzsc.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/giazreboi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/ghegrbpex.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/grvjvxypw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gbpcgdkge.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gttjncjbg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gakgahxie.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/goltuptnd.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gswffjybd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gvmgwhfya.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjocbdgjn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gxhueltir.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfiraqwek.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvdulpdzx.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/ghclkzefe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gqguhxvko.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/ggdzvhsaw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gjqqsbeyw.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gvjnmcekj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/glphpfgxz.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gtnifdpfk.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gnimyxvti.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gsvyotdhj.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gjbocbaga.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gyrgazkjl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gtnpoyitk.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gkwbzbzxs.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gehuovxpw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ghxgkpttu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gsrtvhvxy.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/geemmmkut.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gsjqvjhyh.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gowwkxifr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gwiypcijx.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ggalniwcq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gdmogthmz.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/grocgvjdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gaaesuzxw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gotenhwrq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gibfxviox.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gcoqtdpuh.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gmutouvyy.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gzojiqopq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gueuqhehl.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gqqsmcfpw.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gyqzztrzd.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gsbhjvnam.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/ghresfaqy.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gbninyohe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzbazibg.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gimnjpkqh.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/ggxtvvwms.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gvlnbszgr.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gjwuxjtbu.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbgfyxkqo.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gqwrzkcna.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/glvtmxvtl.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gapnctutn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/goccbqxke.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gkysraeel.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gjsiknxfg.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/ggkkspmoh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/grlnubkaq.sHtML


<!-- 参考信息 -->