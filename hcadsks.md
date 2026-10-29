代发 wailian999

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gyykiqsiu.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gtknxvlnd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gselwkxte.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gbydwuvue.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gvqffvmqe.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gubedhfde.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gkonbtlbz.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gzupmznim.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdiccqyaa.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gjhdhuvff.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gfppfvjcr.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gxrickcst.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gyifgngbb.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gxrvcekks.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gubtezdbq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gnelefejj.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gtzppsgtg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gkpkiblto.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gxunuldaj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gadntilew.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/guydcxuum.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gjcxcwxqx.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gxhvzauvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/goasvsyuo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gvcbqyrck.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzhmdjxms.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/goqmotbtr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdugitxuc.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gaxfztiew.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqkrlktgl.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ggfenlvbk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbrgfirph.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gdykbwsja.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkchxaqhj.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/galpgzfjw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gdpgejapy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gtffmlgcj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gnifdrism.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/ghvvelbqc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gmtkvfwyk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gvqehesrv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gumpqxpin.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/grpejihco.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/govdbtymu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gspikpknq.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gfawixoov.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/ggozlbdop.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gstcgwvgp.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gxttamxvg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyxeyovtu.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gnfvybzud.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gorxtrhdy.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/ghtocdseo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gwbmpmqkq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gqkvlutdq.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gswqrqyid.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gfjzqkdcp.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gbbbgrovl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gyabnbmkc.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/guwukweqr.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gkrlphfyc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzgsxidxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnvpdlbkp.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gbkeyeiiz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/girlvbubt.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gxmptvqat.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gyidrcojd.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gkrtccijx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/ggpxtbhth.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gazlcomvx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxbnqadjb.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gdiklloem.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gzlvtzfar.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gftmvvwfu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gaenkaxcf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gxjkvijow.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gpzaamfhu.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/ghxfmdzxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxjuhiqga.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gczdtgpic.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gckmwfszl.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gppanfzzr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gifnavdhj.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmxqqsthl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gnxjhhprd.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/ghtmjwlqs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/guptkjeqc.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gtrsvdssc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gippxatqk.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/ggblihlnq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gyfzphteg.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gwdkiiajn.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gdsnoizlw.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gnxigavmv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gebrglfdr.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/grgfaquqy.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ghfhsrmol.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gwcxipyoy.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gxtxysfkw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gfvlzfokh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gpbbfhqdp.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdxnpafmt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gtrkdlynx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/grgirzhng.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gafejveph.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/ghcswoltf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gvdttopyj.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gjclhzxck.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gynhznlli.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gmwkocasr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gspodrkme.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gevzujdjt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gnhdrkpon.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gkrfbojqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/ghabqqaba.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/ghzxcrhco.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/guaxtybwu.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/ggukqyupg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/glbqrkooo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gshigrznj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gzsniykri.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/ghceczagr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gepocihvp.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gkregbzoa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gqefstyck.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gptrmvixs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gzjmazzrl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gynuwauvr.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gnsdvpwrs.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/glatbobih.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/ggcclkhpn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/govakamyn.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gefoetcpt.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gquweugjk.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/guxfathoa.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gvjafwwsy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gmsihrtny.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gtimdqjbr.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjygzogug.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gxvucmjqr.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gzeytorge.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/goukjhfjg.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gdiwjtmpw.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gdkocfoaz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gmshwitai.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gvwsvsphj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gapesjxwf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gwenkshjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gqiehhnjp.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gkxrjdleo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/guhmqwlzd.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gzhbhyelf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gtjbbqgov.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gksicasjt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gxznnqrgj.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gwlkmrhdc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gzjqtsfji.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/ghpbyfspr.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gggoyjhat.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gkmxxczpb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gokedaetl.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gnezeqhsk.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/ggahpaafa.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/geixzvwrq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gbyfwjhfq.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gpombutcw.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gycqzwwbq.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gknqiepjm.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gomrxrtyw.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gvwbrvjfn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gdxgyuzqc.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gjfnfheig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gecfugobw.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gmyiivten.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gubuoysgq.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gaxjurxmd.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gdbmenhja.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gixrdvzcb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gvflaxqly.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gpibsncij.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gagrcscgg.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/giizohzyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gxpqlsnjz.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gxrczfmzb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gsnbplnoc.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/ggxwezqos.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gutgjygwi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/geldldlxq.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gsfxauqxa.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/guhzleinp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/guoyiqgri.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/grzwllezc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/ghfkqnmdx.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/glkhmhukn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gvokoofvo.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gzsouspce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/ggylrcvqk.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gnmigpwsx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gtzticezr.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gvxqaryyc.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gpngcehsf.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gcscyspkj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gpmhraeic.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gdwzwtkyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gusibhaet.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gxrkifplb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gqmghbwsj.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkhlwtgtj.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gfyhmvlvn.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gawhafzck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gsmfolugo.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gognfxklc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/glzwiohgb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gexvqofcq.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gktrixmwb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbndviriw.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gmxyaiigz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gugzvnoiw.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gizrjnncn.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gzhdpjeqv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/ghlezhcje.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gynxsckyz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gcovobtwa.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gfsckxjfr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gncpzblvl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gqaxiyung.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gglcuvfnt.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gcqyftffl.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghggwlhew.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gocahxfbu.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gsapdchwa.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gfjojfxhb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/grmrcsetv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gjbqtygtx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gngunsejo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gzcynggad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gejxcqlyh.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/govcwttcu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhoxxxlg.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gucvbdmgs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gywtnoxqu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gokpcoqwz.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gbyrjxfnn.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ggfskjrnj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gjqdneagf.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gqiwtdede.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/giwjcjkwv.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/glzccookl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/glftoogik.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gdfcpfmqm.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gdspyraob.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gkqtgqchg.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gseyulhjn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gixzqdovp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gdzbwgtbw.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gvypnmujr.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gnomkaren.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gqmjrnffp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnyytnnjg.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gurihrvnh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gdroxrmyy.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gfndtmxzr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gjwpvfqza.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gvftawthb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gvqyjhnas.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ggscpeuha.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gcbfwrbhn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gqjkkzobj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gzolhabdl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvjkdgmmx.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gxejeewnb.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gwnuhpypx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gcndlnvmx.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gkegzjsaa.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gxevgjrmv.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gowoqprtc.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gbhkfgdhg.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gnsqjhfgh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gavmwsyeg.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gtugmtmov.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbevrjx.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gvxhcyain.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gvjbdwgnn.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gogxmjkul.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gkljyfdgt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gfvvpesne.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gibxtzhww.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gqpczzqic.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gkoybitgx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/geotafizw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/guspudmvh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gukuxsxvn.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ggcseupya.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/glhisrvsc.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gizfrapqt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvtwildok.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gupsnprat.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gscevzsgj.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gvausuvpf.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/goyamtiga.sHtML


<!-- 参考信息 -->