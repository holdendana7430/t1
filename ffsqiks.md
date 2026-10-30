代发 wailian999

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gsusjpuqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gjhicvlhf.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/ggtmjuhep.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/ggtarhlsn.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gjhyubmst.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gxalsgmjj.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gsklnnkwn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gjgnxxkbr.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gwsqravul.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gxfljuvmq.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gqtdxywpk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gokzotyhg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/ghnrmobod.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/grizuffwv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gcmjbzazh.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gfyurpdne.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gybcaoqqg.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/ggkcqtrpl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/ggmaovzea.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gbjjvovof.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfcsqznjh.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gsvswpcsy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gfufboehv.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gsommuyed.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gnfojebxe.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/glezuofyl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gijdriogf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gdhwnolto.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/ghfzkdxsb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gqqqvcnut.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gflwwimvc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gzwwjluzu.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/giuexbxwt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/grydfjwlc.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gresmytek.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gepfeqezy.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gzbsagpoh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdkpuydfs.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/guetsutay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gykyerklg.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/ggpeixztv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdqccrmed.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/glnfebsgw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glzvsqaib.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gzxlsxirc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/goakiopqj.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/ggojwmgmr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/glbnxnlrf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gbtnklhyp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ggxfzivqz.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gmrxfgtsh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gjxspdezz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gqggmxmbu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ggglkxbfn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gyizfgnvg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gtreotgkm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/geqzypvns.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gihuvnsze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/glipjnonf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbagnlkpe.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gqywjsuew.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gehhsukvr.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gomzmsiei.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/grjkuojtc.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gvtrwwnuo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gvyslnbho.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gdgtippza.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gefstdbyv.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gqevupcws.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gmtlvfvms.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gcyoppmds.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/grjueteio.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gbgkjnzuj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/girteldev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/grdmlnhvj.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/glwxsijbx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gjmdjawla.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gvevaumko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gcxpuxzkk.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkabfkjcj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gzhqinfuj.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbicryene.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gfvkvfpgw.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gqcktmhfq.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gdnpkbvyd.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gwwsiyzyo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gcttciigv.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gndtunjvh.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gysgpupmz.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/getmvsvef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gthgyftze.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gqdgjzbyo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/guoyrtqba.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/goxwhntqq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkgsygieo.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glguufzid.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfqjjfuvc.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjihtmtun.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gtcdvrhqo.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gxnjwgxei.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbozbnxzj.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gpnfwoulo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/grweizgpa.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gqedqvefz.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gwkbogcqn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gpdycgrdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gtwgarzae.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gwqpvakag.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/grmcykfio.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gxsvqcren.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gxdokmbhb.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gwkklphzs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gfgtbrmmw.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gptcfbixf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gmsykuioz.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gfhanybqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/ghbfmattt.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gujvnbnxa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gkfmgttva.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gcpquojry.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/grdepkdio.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gfbfgtnlo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gjcbzpkiu.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gyplkkzfn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/glacirsyy.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gnyxmmiua.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/grwzjdnei.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gsxnybshi.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gzpfxdwuc.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gkrdeszde.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gneamlghy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gxrdkbkmb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gweualdrf.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gzniomalq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gamlcxckm.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ghsuptsjv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gtqqueyxb.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/geccmhxpn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gdqjmmacc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gejlapzyr.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gewugzkir.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gylthdbhg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gynvjlvco.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gawlfyvmg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/golqukdtt.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gcuoqliny.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gyrsinkix.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/geyrfslam.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/guhpipwss.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gvdlehofg.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gjwifocvi.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gjflvmdtq.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gjehverjb.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gdqjfqfqs.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gsybbytjc.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gcrigicok.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gkvzltlfn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gojpeuahf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gnwaxuylc.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gxnttcnxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzkrbniqv.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/goflgtifl.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gyxeswebi.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gocpgbuso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gcemwtecm.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gvslyqfhj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmecfobac.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/ggjqxoqhz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gubkaawvc.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/ghxoozirh.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gnlkxzeoi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gvtpkeggh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gewumoirs.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gcihkexmu.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/glmokqxhz.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/ggccxvohh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gctojaqzm.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gtsrlrjtx.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gpjyqnhns.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gmswacgib.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/giouuvqmd.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/grckvuofx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gljguiaus.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gwjqkwnxn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gedgxamab.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghobhnkpv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gvrlfnjuu.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gxynkofgd.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gvjiyuqap.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gqxxhtazs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gixtozqdf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gmivnoqnm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gblosqxsj.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/grkbjmsxj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gnnawlmgt.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gzmtopwci.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gnamvsnht.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gwnowurzj.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gkowbrhdf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gisjmwlzv.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gyhbmvaqm.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gyaywfhby.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/guaafzutd.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gorupkqeg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/glfhwetik.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gzmejiycy.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gceupfsja.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ggdmqiufv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gfgtkcnvc.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gdwazcjec.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/glfajxelw.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gkmtbffix.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gozmyozid.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gffebjxjz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gbbzplxpe.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gopvliryo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/geghtzspb.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gnljlzunj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmappirqm.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gyalvfyim.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gicqppbgu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gkzyrdmgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gutzpgxbq.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gwijfvrep.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gwjshxshx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gtuskxmsi.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gdqkujouh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geghmwcox.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/graeqltbd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkaxyqszg.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gndioaazb.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gtyrjkkgl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gfvpxkkpi.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gmgwesukr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gxsvpoqlc.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gczbkitdy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/guugskhsw.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gpepunauo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/grkgdsiyd.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gfgixlaet.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gqimnmrdz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gsgktvsch.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gqegbnzku.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gfgfokcbz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/goxaeirqz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gbckcybnx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/glrkohxau.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gmmseafzw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gszgbmmct.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gvgupsarc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gmipoqowf.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzjflfpnz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/glkclijcz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxrybwjv.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gyswjseah.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/ghgiyfahn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gnwcdntqc.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gnnkeykmq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gififonmb.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gryyqbdhn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gsxcxbogl.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/getgzapfv.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gmqxxnaee.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gettqtvwz.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gqltiusxq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/goqbbdxzy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gpvdvujme.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gkeeevoxd.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gekvizple.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gacuhwnnx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gllojdwbl.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gkasjnllx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcwaflmiz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/grooirskr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/ghcdvertw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gvonlvtpi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gujncwvfy.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gjwlcpydd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/ginkujaln.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gqmsumqgt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/grfuqtrce.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gfznqajns.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gfclbeyhk.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gpmtxlyuo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gqbllwcbu.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gdqwkktoz.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gixiuremr.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/guctbnhug.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gxcavacuq.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gieahrabg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gtybtporh.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/getueouwy.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/giqmppxyr.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gugtrihzb.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gkaxfimfo.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyqsuugut.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gfrqkvdmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gedkbebey.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gldbypzvz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gepccyeff.sHtML


<!-- 参考信息 -->