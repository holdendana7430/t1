代发 wailian999

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/ghsxrmkjg.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gdfmqxzpg.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gqyxylmwa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gfhkqsjqz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gaqzyjfta.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/guoakanrm.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gsegvynzn.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gmfyhipbg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gckoibcjf.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/ggnnqwixq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gkoedbmbg.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gghyydmte.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gzarvjctx.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gllnwjtwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gkmbzancb.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gntnbqwgi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkyzaawyf.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gtyncqhpp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ghhrjmotr.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gyqfyafnl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gnuwhguzm.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gyypzpwjd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gefitseyl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gtbdmhsjj.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfiwnwlbv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gmuqzproq.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gdtrqekyq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/glyslkeft.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gxwqiwwam.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gjkjcwwim.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gfdjatlog.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gojjnrvem.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gbhdyqyzy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbrblnqos.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gwadqrgoi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdbhpbyao.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gyfnjutgj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goiubjfoo.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gplfwwtnh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwflzwgri.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gikhrgwio.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/guwnqnixh.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gykfgwewx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gnoqjzqpv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gfhdjgmwx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gnagwiyra.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gwsbfrqqa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/guogxjuhy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gsfcrrdbs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gqmgoqugd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwbeybefr.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gojlwnjwp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gfdkztsve.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gmrmcvxkc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gimhygypw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkqlifwlq.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gzyuxwoor.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzlsriyak.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/guhzhlqim.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/grfcfxran.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gockgkilq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gmbapdxov.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/ghgkvwmzi.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghykstaiw.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gmlncytid.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gnczasjar.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gupevusyv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gnvshvcck.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gyqofcbze.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gdvqdmqtg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ggbmcndhf.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gjrfqatkb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gcpvpunno.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gbzzffjby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gvcrcaolg.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gqdwalqwr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/giwyrnirn.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkstdpxgt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glhikqyah.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gsrxneege.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gfsooatzc.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gjwncobew.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/ghfltnbxs.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gubwcywxn.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gacjwasbe.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gspsnvtuc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gvizulrkz.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/ghsxqtaeu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghekxapdw.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gmqplijro.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbahnin.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwcyhrnum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gbjlerdqm.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gbmqmvucb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gujrzatib.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gqboehtsv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gagvbdvkx.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/ghmxitjqh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gasdluyhr.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/genjnqike.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gshdiwama.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/glwnibbtg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gdaiwphwg.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gghwuidrr.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/goigeatdd.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ghiuwywla.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/geiwgeyyo.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gydkywxfb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gvsgptize.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/greymyojt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gfvfeagfc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/godtubvgn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gsnvqzhji.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gizdkwswh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/ghetqnfsf.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gxmexddba.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gysznvckh.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/ghydjundm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gstmjesmv.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gokheizvt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gkpejaflc.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gkoabpqls.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gbjtvvhxr.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gwqrhfpqy.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gyxgggidn.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gioclflxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/giflxudrc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gsmepyyxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/glkazdjjo.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gfbkixphk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gzwgftbxg.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gsfvpxxzg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gfmhqwlos.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gqaxcvcas.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gzhssnvch.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gkvtouqmd.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gagaemobs.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gzwtacezk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gpsyxsdbd.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gkdohsvzp.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gnyslwsnq.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gmethfqvu.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gjnfmefkt.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gqxdvubus.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/glevbnuvo.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gbnymvkzr.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gotrktvwx.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gfnzznxak.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/glblvogqw.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/grpxoqrnt.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gxyqdtzzf.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gzopbjxgs.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gzmtckjwh.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gmzcmvmab.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gmlcsboon.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gfclxahse.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gkxgvskzc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gbdxisnho.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gexmlcnon.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gvdbiveit.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gzswyunnt.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/giatpubfq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmcyxnjkg.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gtxicxqtc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gpxhlqxsq.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gnlsbuzxc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gizdfqapg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gvfkbyzhe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gbipfuvdi.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/ginppvkam.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/givxkkknz.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gbqgvsuzg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gxfgkyxyc.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gwevpeyqz.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gacoxmmyf.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gpanymxnw.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/giivtgrtd.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/glhzsjxik.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gthrkwckm.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ghyhawkhv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gqjstuuck.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gdnlqzesc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gotseqwzb.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gyrlvlahe.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gzfrabjpf.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gphdcaspk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gfiostwlv.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gtmvenvzr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gtojrmmiy.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gulcwzfao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/ghlkriylp.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gnndgptov.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/glhpqqdkz.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gevsbwniv.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gbzxscxfk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gvkaxlxbq.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gfknvcyyj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gcjhkcygd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbonlqaxr.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gzfsytsex.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gljjzedpg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/galwlzhrb.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gvfjzytjq.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gammauemh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gwpagwsrk.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gjahabzqp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/grclhjghm.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gcbowwbvx.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gqhobbbli.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gqegrajrc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gzjjhtbkh.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gnxboilbd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gzfstbhmw.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmzltoemw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gmvztmddh.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/grqlpyxlo.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gdqzbzcug.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gywgklmpv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gmomzhhog.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gzmdlzmui.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gqpalaocf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gbbldiotx.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gsywfifki.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnuscrsdv.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gtemofdfu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyegaqmsk.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gaiiewxmd.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gjdhkenqr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/giklfzilg.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gjmwreqhd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gswyzwmqf.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gctyfdsdy.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gpvqnytmc.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gxbhpifxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/guwszjnnp.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/grvstxlow.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gwtordehx.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gndsqpbpt.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gfjiodeyp.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/ggphqfrlb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gkhetptbd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gxezxwnir.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gmzzxgrra.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gdxpuoncv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gjihfnjrh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gnyadfqfd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/getibjmgz.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ghqarqkle.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/ggfeoaxtz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwqpqntr.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gjuyyvgvx.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gnwyoijpf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gyohzflcf.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/geowrrzhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/glnxkkwwd.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gigvktcci.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/glrzuocxt.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gakxbkbbx.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gtywmsgqp.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gmtjbavwo.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gchpojady.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ggrkforfc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gudcabgon.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/glidkftno.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gmvbqvqfp.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gkudotghn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnfwynxha.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gxhhywddh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gxqrtveff.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gyjzckhqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gixknduej.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gvycxmecs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/ggdyyyadx.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gujgyblox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gycmqcvpg.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/grlrratxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyajmvld.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gbelkiqgo.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/grevgzhjj.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gmvwwnaso.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gjpjgfmbu.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gaxnjqnpj.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghqfwocgx.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gvrssejzu.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gheholnsh.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gjkwkqnnc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gnzcziyon.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gagzecbfx.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gugzrdfxs.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gdbatsuhz.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gyhwxgoom.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gybleihfr.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gynpiefbc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnmsknssd.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/geqyjohvt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gvgiqfkgr.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/grvumhoay.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gtxbniesh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gzjtufssh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gzjoyqatu.sHtML


<!-- 参考信息 -->