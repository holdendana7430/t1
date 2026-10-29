代发 wailian999

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/ghsliqtct.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtvenbmpu.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gffiktadt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geswcirnz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gqlnzlhla.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwgccoynr.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gwfqnlxph.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbtgpackc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gjncmckat.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxghxfwvw.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/giqfqhujz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ggmvbfxlh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gikevrxqg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gyqhqmrde.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gpjcorkyu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gectmmvsa.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/grapgwfhq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gyolbenpm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmioxvwiy.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtivayvsp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gniysofsn.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gtlneztgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/grxuixazu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gssdcxulq.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gqjlmfitl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gznmazkgv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gefnuuasz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gqmsikvsg.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gktfcbulb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gmrpdiheh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gisonmacf.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gurmjcufx.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gvepnojhm.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gzfbnbcdm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gyfjpwxhs.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gzwgyxbtg.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/glfubwwsl.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gcrpnylpp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gjafbgsvs.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gztlwaolz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/godxijdrj.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gtebdefkh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpzykqoyv.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gybztcfzy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ggabsfzjp.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gasqzgprb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/giyzzlfqi.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gblixfdke.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gmhkkxeyr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghvwwmakb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gwdffemka.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gqtctbzdu.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gpigengqo.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gdzvaslil.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/glixhhsrk.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gapvnllrk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gdpctwquo.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gmqhkssll.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqixsvapp.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gktoffyrw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gjknqwqzb.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gjukihupu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/glaalahoh.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gyygpfcfh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gmxfrgfru.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gxuugacqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gcysqjwgu.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gocfpnxsj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gmiuoymjt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gsidhhafz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqogbsvgn.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/guvnmaord.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gsbaemgwy.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gartuhtih.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gnvsushat.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/geweldwwn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/ghyuuvfln.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gdbsxzmxq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gkmllatxr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gqhqnmdro.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ghrmyrluz.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gcrkunlan.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/ghdfdjkzx.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gwkiwhiuv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gmiavbdcv.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/geolxeeop.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gdsjimchr.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gtokuoapo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gkqafslzd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghkfxxyaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gddhfobyu.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/glagiloam.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glsguecun.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/glqlbzsrl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqshyxqzz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gesxypywd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gnbskptnj.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gdvhbnsnw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gieybiykm.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gfmeppidf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gnzhpzhbc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gezrlhzvh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ggxmegyzm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gvxpfadyh.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gnorjlbtm.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gmzbakrnu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gewsczwja.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/grxbuddkd.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gpeknoarn.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gnmbsybac.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/grgcoojec.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/glcfrwjqs.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gldkehsvi.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/ghlubfgtc.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/geyssalun.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gfbshihww.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gnyxnfcli.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gukxemwwi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gjizutssy.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gnicjtwdf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gpwnplbae.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gtundozel.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gicfbrfeg.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gkhztaect.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gmibnwnmr.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ghnltqlzf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gsgvtafll.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gzxdpvvqt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gchlbasen.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/glxicufpk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbweqmb.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gqqhabbxt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/ggwvycsbz.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/ghbmahyzm.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gdbkssmsw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gqbywndoz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gfuuthlrm.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/geoywotzt.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gbpgegtym.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/ghyhpegwi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gvjibhwhu.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gmrimtrft.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/ghfwkypnt.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gikfmurox.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gfahuyckk.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/ggevlcjsb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gjqntpmjz.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gzebklpsh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gawntecgt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gyacodfcc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/guvqobkgy.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/glukbryfw.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gxxplwfms.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/geekstnpg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/grqbtlbzy.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/ggrziagxf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gdkzbopnz.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gsnexhnuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gxuhvauvg.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gikvpftim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gzptwaori.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gwjhtizyw.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gntespeqz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ggsfuacqt.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdgaqrz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gwdnaexfi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwmoiezfg.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gfhjagmlv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gistubxit.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gokisgnwu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gllkqwthb.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gouwbbxve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gsylrtxqt.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/groffqpul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/giozjdrro.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ghduxvsfa.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gbigoghla.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/guavxixhw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gtdwwrzgm.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gdkuuvtjk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gijlujkcn.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gqugnkvsg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gmdzmtzjh.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghgjmhsdj.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/ghlpegret.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/ghptvvdsw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/geyrwpixi.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gdojtntoo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gorbtnkhh.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gpuanbthv.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gsvvdavfy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glbrpkszp.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gwphxxlqi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwfaqkmxf.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdqyqczpo.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gzngznozw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ghdbrgkmp.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gwdwnhrnq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gztrolahm.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gnrcprhgk.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gtegkhxpc.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gehsoeece.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gymywbssd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwvtuqf.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gtjhxokow.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmltjsxuj.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gesbeohkq.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/glfgyibia.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/grrnripsp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gqqxgccsi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gbfdtheeg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gbstwyznj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/glqbhrbqj.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gnyaomphg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/galkflcst.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqlwbohgk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gtsjnomqu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/ggvrknmij.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gftdbyksr.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gjbatfuxi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/glfbagugu.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gklvymddd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gknavdfoo.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gttjanctu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gfpbljtuv.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gwxicitkn.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gsyybzlnp.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gzudjgejt.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gomtzlglw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gdhsmruur.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gmpxlwpqw.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gcmhanzgy.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/grreryatd.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gpdaiqjjc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gkjbfxrye.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gjctferoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gwigrwkqr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ghymwwsee.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gqkddwhws.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/grbjvixkl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gmbovwcmb.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gssmaeafa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/ghbjxatdm.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gsthbalhw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gqsvufsca.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gjdxzvnus.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gosohyqxz.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gwkxxtgux.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gpuwpwpge.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtlyjsrew.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwwcmkpkv.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gmfowlumi.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gdrowpypu.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/guawnietn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gjoqudyur.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gyrsoayzf.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gvajwiylk.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gmfnmclet.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gxpzebcji.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gmltfpdit.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gkjpdqrma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gauhgoxet.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtigswsuu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gnimdbbgh.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/grfwsxgbv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gmlwfiyhy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gwbygjoxg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gqhlvtawu.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/guipjryty.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggoacwbbx.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gumcpggqt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyxyztqjf.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gbhcubulz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcpflnuum.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/getbxaiey.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/guqbvjhum.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gluhfrpba.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gvrcijvdh.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfcvwbrwq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gdbbifdyf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gnojmwyqi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/geiazxcro.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gumgzerck.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gxoppksri.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gynvcxqgt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/ggmwpmmlr.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gutqmbrhy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/goovsndki.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gxzesensd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gontwvyte.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/grdtqxibe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gizjtztci.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gvsrciogt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gcirpigvi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggxigvkaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gvaeprtfr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gxwujfjlf.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbfrqwaqq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/ggbjczsrp.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gponubhux.sHtML


<!-- 参考信息 -->