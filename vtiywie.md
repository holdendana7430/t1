代发 wailian999

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gvuivjpkv.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gvhvpccax.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gjwdwnvzh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gxevwzbln.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gbuagqwqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ghxwyauxd.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gwkwyfgpb.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gvjxmepsm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gnsfxlmxf.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gmsimvzoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gpidmjmom.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gikdoljui.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gemgtllrb.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/glfgsvqkx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/goksgmqyx.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ggftbjfma.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsclrumqj.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/ggwqgpjsc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gnjyretke.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gcbwzuwtk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gtiealdly.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gqypvsogt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzpjpmilw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gctaltsha.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gsxwqualk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/grlrgymzm.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gcagjvvwm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gvsmmxxol.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gpcuubxhq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gufxskbon.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gqmhxklsm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/grnsxiick.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gfdzywmtt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqtoxculu.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/ginkmxtqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxdyrzvvt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdqsgpehu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gewelkvwc.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gknrevfdx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/goinkvxyu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gzyqethzg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbunaazco.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/ghevxkbul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gckoawtuq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gocbzpawo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gflhtpqxr.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gmraslkdb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/giocqcxuc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gssrhamkk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/giaauxnlr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gmnbglbyn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzzqbofsg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gqhvjovoa.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gszrbomoy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gbmeudrwy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjphlway.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ggfvhmleh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyscofchr.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gdtjygevk.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gvkbwjevj.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gflpdrejd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/ghnzkprod.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gbdfmhznd.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gvcfypzad.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gypdtqgnh.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gjihqocff.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gxnicnqgm.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gwpydmlmc.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/genmzrgbl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gyzvoqmyr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkekbpjzk.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/ghlnkkfxe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gzbgrcpxo.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gmdbpovug.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gleyzumwp.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ganiruukv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfrumgifq.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gorjyuzsl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/ghyghynwj.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/guymrvymj.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gnqkbgzae.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gijlynhuw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gbaaieiyz.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gcweyvkot.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gbhtabmte.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/geqjbenhd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gcfndndgu.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gagcjketu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gxwwlspux.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gvquufklw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gzoysnlyw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwanrqdwc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzooyievd.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gedjnxend.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gamzdwqcq.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwkdjmvxj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/ginzicmuh.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gyjwhhhgl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gvzvaqzbs.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gfmvcykrh.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtkvupcgz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gokoymsyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gczvsemnw.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gwwapgmuw.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gactxmcux.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gugvjjhxw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjjimrtkz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gbhzcfnjr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gtyivmnza.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gvzchhfho.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gomvywjyt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gglkjonmv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/guhsdozdu.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gmapttikl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gvrehmmel.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gvprhdjaz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gwdmfqyfc.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmszvaydw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gntexuhnp.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gjfudpoxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gsjamnpcf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gwrqajazi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gkolyipob.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gxfmtpqcz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gegbozarp.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/glqeeeljy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gdxgxlhlf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gyvewxonx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gempifzgx.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gxovamalq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gurmcndso.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gmwebktqr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gafteecbd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gpugydaam.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gmjuxuidg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gkqrupmym.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/guauexgfu.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gyxfzwpct.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/ghwmovgnb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gatcwumfg.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gcbkuvpke.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gjrftcrml.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ghhorkiex.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gkpimalmq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gawuejhrr.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gacymwqbr.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/ghuwbyyuh.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gdmyijvcb.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gxbuyhruj.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/grchlljtk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gkzvuqgny.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gdujceuti.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gajssoszl.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gnokjjsmi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ghadobwih.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/greawmfjb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmhiqpqns.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gwiqlvmwc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggpmtxdjs.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gdmwjvzze.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gslxhcsxt.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gwbfeiqzy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gwujuorwt.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gxtkgqqsu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gjrhktbnz.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gpibwyqls.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gslekcazg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gsybemuoa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gdscmgyla.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gcaqglzls.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpdlbkwxc.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gkwmoofbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gxxcberxk.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gvctggitj.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/grxfhstex.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gccwrxrhj.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gjdmpycjq.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gwdyxhwxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/grgtilrtd.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwbywkocs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gpntwsxjw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gberuhazd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gicfxpnrq.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/glkbijtfu.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/grhtwzqmc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/ghfutsqjb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gfixdadhg.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gjwicukjv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gkvxltdjr.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/grurxwlii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gxtpxhoat.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gsmudxuzx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gohtzdfem.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gifwssrad.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gmobmjqef.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gxezvpgmh.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/ghhvaqvos.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gsggyoqup.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gykujwmvu.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/ghqeymbtp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gacwcrlzy.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gpucdsewy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gkuniypac.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/girgmttaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gelszonfm.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gabbxrozw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gexousbrl.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/glzndgvyo.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gyloflhgh.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gbfyxdujh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gxvhpdhho.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gvcbodcst.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gltkkhcvu.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gwyhplnio.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grggxyjst.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gsdbnsvve.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gkwgkxnpg.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/ghzivpodo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gzwggxldt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gjnlmzrnz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gwdnjqjhh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gfhuxcuwc.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gclbfccbb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gajobhpbg.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/ggbsfilhm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gakzhotze.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwbcpkhyq.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gulkqkkfm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gjipsvizx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gidwmzcfx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/guegqawvs.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gsljhhtxg.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gzxqxwuff.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gtnquvhjt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gkhlfvykp.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gmqafkuon.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/glvndeaui.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gctpwceou.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gukiqyqic.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/grasxrktr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gcjmbadvk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gqtwbxavf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/glhondjqk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gcutbmdap.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqprieu.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gfgkghrwn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gbzrenalb.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsmtickuo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/ggpustref.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gneuhycfz.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvzeentu.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gmavigper.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gzhknljrl.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gbwtfrwvq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/grcgdbvhs.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gjrfulqnn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gzmjzxqon.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gkfmstvar.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/galftlkkg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gvqnbzutz.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gvgtybtwo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gqgsyrzut.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gnnemkevf.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gmzahxvdz.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/garjutsxz.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdzesdute.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gjdhbanpf.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnoooagiw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gwphbixxt.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/govqiogpp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gdaaeuudq.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gconnamld.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gpuasevpu.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gtxnkqdsw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/golmxskud.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gqnlhqkdr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/githsowhd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gtygoxftc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gopohrunp.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gdaptnddf.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gdnvjsazl.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gljjalpeo.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gasnmoyzu.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/grheeabxf.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/ghkzigjvg.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gqgfclduy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gfdrswqjw.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gnaohtlpc.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gqxnjgmbw.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/ggjjahraq.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gghhqzhqn.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/geemxfnec.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gwqeygksy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gnadrckjy.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/giynvivvb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gcjgjegtq.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gwsfhcddl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnjgdzwqj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gsrkmirth.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gdxbulkhq.sHtML


<!-- 参考信息 -->